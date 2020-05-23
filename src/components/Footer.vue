<script>
export default {
  name: 'Footer',
  render: (createElement) => {
    return createElement('footer', [
      createElement(
        'div', { 
        class: 'container mx-auto max-w-screen-sm -mt-2 pb-4'
        }, [
          createElement(
            'p', {
              class: 'text-gray-400 text-center',
            }, [
              'Garage by ',
              createElement('a', { class: 'font-bold', attrs: { href: 'https://coderdiaz.me' } }, 'Coderdiaz'),
              ' / #keeprockingwithvue'
            ]),
        ],
      ),
    ]);
  },
};
</script>
