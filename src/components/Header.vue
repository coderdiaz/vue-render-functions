<script>
export default {
  name: 'Header',
  render: (h) => {
    return (
      <header class="bg-indigo-700 py-4">
        <div class="container mx-auto max-w-screen-sm text-indigo-200">
          <div class="flex justify-between items-center">
            <span class="inline-block font-bold">Suscription Tracker</span>
            <button class="px-6 py-2 bg-indigo-500 text-indigo-100 rounded">New suscription</button>
          </div>
        </div>
      </header>
    );
  },
};
</script>
