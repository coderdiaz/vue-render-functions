<script>
import Suscription from './Suscription.vue';

export default {
  name: 'SuscriptionList',
  render (createElement) {
    return createElement(
      'div', {
        class: 'py-6'
      },
      Array.from(Array(10).keys()).map(n => <Suscription amount={n} />),
    );
  },
};
</script>