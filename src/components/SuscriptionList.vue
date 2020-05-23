<script>
import Suscription from './Suscription.vue';

export default {
  name: 'SuscriptionList',
  props: {
    items: {
      type: Array,
      default: () => {
        return [];
      },
    },
  },
  render (createElement) {
    if (this.items.length) {
      return createElement(
        'div', {
          class: 'pt-6',
        },
        this.items.map(n => createElement(Suscription, {
          props: {
            name: n.name,
            description: n.description,
            amount: n.amount,
            color: n.color,
          },
        })),
      );
    } else {
      return createElement(
        'div', {
          class: 'border-2 p-6 mt-4 border-dashed border-gray-600 rounded',
        },
        [createElement('p', { class: 'text-gray-600 text-center' }, 'No items found')],
      );
    }
  },
};
</script>