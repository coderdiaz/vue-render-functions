<script>
export default {
  name: 'Suscription',
  props: {
    name: {
      type: String,
      default: null,
    },
    description: {
      type: String,
      default: null,
    },
    amount: {
      type: Number,
      default: 0,
      required: true,
    },
  },
  render (h) {
    return (
      <div class="bg-indigo-600 flex justify-between px-6 py-4 mb-2 rounded items-center">
        <div class="flex flex-col text-indigo-100 font-medium">
          { this.name ? this.name : 'Unnamed' }
          { this.description ? <span class="inline-block font-normal">{this.description}</span> : null }
        </div>
        <span class="text-indigo-100 font-bold text-xl">$ {this.amount}</span>
      </div>
    );
  },
};
</script>