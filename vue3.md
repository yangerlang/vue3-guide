composition API
1. reactive
   const { ref, computed, reactive, toRefs } from vue;
   const refData = toRefs(data);
2. 生命周期
   beforeDestroy => beforeMount
   destroyed => unmounted
   onRenderTriggered
   onRenderTracked
3. watch([greetings, () => data.count], (oldVal, newVal) => {
   });
