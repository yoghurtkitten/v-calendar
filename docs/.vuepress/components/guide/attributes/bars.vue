<template>
  <div class="example">
    <v-calendar :from-date="new Date(2018, 0, 1)" :attributes="attributes"/>
  </div>
</template>

<script>
export default {
  data() {
    return {
      attributes: [
        {
          bar: {
            color: 'red',
            class: 'my-dot-class',
          },
          dates: [
            new Date(2018, 0, 1), // Jan 1st
            new Date(2018, 0, 10), // Jan 10th
            new Date(2018, 0, 22), // Jan 22nd
          ],
        },
        {
          bar: 'green',
          dates: [
            new Date(2018, 0, 4), // Jan 4th
            new Date(2018, 0, 10), // Jan 10th
            new Date(2018, 0, 15), // Jan 15th
          ],
        },
        {
          bar: 'purple',
          dates: [
            new Date(2018, 0, 12), // Jan 12th
            new Date(2018, 0, 26), // Jan 26th
            new Date(2018, 0, 15), // Jan 15th
          ],
        },
      ],
    };
  },
};
</script>
