<script lang="ts">
    import '../app.css'
    const data = [
        { icon: 'fa-dollar-sign', value: '1,399,999' },
        { icon: 'fa-credit-card', value: '1,600,000' },
        { icon: 'fa-dice', value: '0' },
        { icon: 'fa-briefcase', value: 'unemployed' },
        { icon: 'fa-gun', value: 'Test - Gang' }
    ];
</script>

<div class="absolute right-3 top-3 text-white w-48">
    {#each data as { icon, value }}
    <div class="flex items-center mb-2 p-2 bg-gradient-to-r from-[rgba(0,0,0,.9)] to-gray-400 rounded-lg">
            <i class={`fas ${icon} text-pink-500 mr-2`}></i>
            <div class="text-white">{value}</div>
        </div>
    {/each}
</div>