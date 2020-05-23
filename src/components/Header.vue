<script>
const items = [
  {
    name: 'Spotify',
    description: 'Family Plan',
    amount: 9.99,
    color: 'bg-green-800',
  },
  {
    name: 'Adobe',
    description: 'Creative Cloud',
    amount: 23,
    color: 'bg-red-800',
  },
  {
    name: 'Apple iCloud',
    description: 'Family Plan',
    amount: 23,
    color: 'bg-gray-800',
  },
  {
    name: 'Apple Music',
    description: 'Family Plan',
    amount: 12.22,
    color: 'bg-pink-800',
  },
  {
    name: 'Youtube',
    description: 'Family Plan',
    amount: 12.99,
    color: 'bg-red-900',
  },
  {
    name: 'Netflix',
    description: 'Premium',
    amount: 14.99,
    color: 'bg-red-600',
  },
];

export default {
  name: 'Header',
  render (h) {
    return (
      <header class="bg-indigo-700 py-4">
        <div class="container mx-auto max-w-screen-sm text-indigo-200">
          <div class="flex justify-between items-center">
            <span class="inline-block font-bold">Suscription Tracker</span>
            <button class="px-6 py-2 bg-indigo-500 text-indigo-100 rounded" onClick={this.createSubscription}>New suscription</button>
          </div>
        </div>
      </header>
    );
  },
  methods: {
    createSubscription() {
      const index = Math.floor((Math.random() * 5) + 0);
      this.$emit('created', items[index]);
    },
  },
};
</script>
