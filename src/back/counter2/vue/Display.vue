<template>
    <div>
        <h3>统计值： {{ counterValue }}</h3>
    </div>
</template>

<script>
    import { getCount } from '../vuex/getters/index'
    export default {
        vuex: {
            getters: {
                // 注意在这里你需要 `getCount` 函数本身而不是它的执行结果 'getCount()'
                counterValue: getCount
            }
        }
    }
</script>