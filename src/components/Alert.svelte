<script>
    import Icon from '@iconify/svelte';
    import { createEventDispatcher } from 'svelte';

    const dispatch = createEventDispatcher();

    export let text = '', title, status='success', show = false;

    function closeAlert() {
		dispatch('close');
	}
</script>

{#if show}
<div class="z-100 w-full fixed left-0 my-3 bottom-0">
    <div class="w-11/12 max-w-md p-4 text-slate-700 flex flex-row border-l-4 shadow-lg justify-between m-auto font-semibold text 
        {status == 'success' ? 'border-green-600 bg-green-50': ''}
        {status == 'danger' ? 'border-rose-500 bg-rose-50': ''}
        {status == 'info' ? 'border-blue-500 bg-blue-50': ''}
        {status == 'warning' ? 'border-orange-500 bg-orange-50': ''}
    "
    >
        <div class="flex flex-row">
            <span class="text-4xl mr-4">
                {#if status == 'success'}
                <Icon icon="ph:check-circle-bold" class="text-green-600"/>
                {/if}
                {#if status == 'warning'}
                <Icon icon="ph:warning-bold" class="text-orange-500"/>
                {/if}
                {#if status == 'danger'}
                <Icon icon="ph:x-circle-bold" class="text-rose-500"/>
                {/if}
                {#if status == 'info'}
                <Icon icon="ph:info-bold" class="text-blue-500"/>
                {/if}
            </span>
            <span>
                {#if title != ''}
                <h3 class=" font-bold">{title}</h3>
                {/if}
                <p class="">{text}</p>
            </span>
        </div>
        <span class="text-xl font-bold ml-4">
            <span on:click={closeAlert}  on:keypress={(e) => {console.log(e)}}>
                <Icon icon="ph:x-bold" class="cursor-pointer"  />
            </span>
        </span>
    </div>

</div>
{/if}