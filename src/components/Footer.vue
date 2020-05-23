<script>
export default {
  name: 'Footer',
  render: (createElement) => {
    return createElement('footer', [
      createElement(
        'div', { 
        class: 'container mx-auto max-w-screen-sm'
        }, [
          createElement(
            'p', {
              class: 'text-gray-400 font-bold',
            }, 'Open Source @ 2020 / #KeepRockingWithVue'),
        ],
      ),
    ]);
  },
};
</script>
