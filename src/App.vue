<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import SubscriptionList from './components/SuscriptionList.vue';

export default {
  name: 'App',
  render(h) {
    return (
      <div>
        <Header />
        <main class="container mx-auto max-w-screen-sm py-6">
          <h1 class="text-gray-400 font-medium mt-4">My subscriptions</h1>
          <SubscriptionList />
        </main>
        <Footer />
      </div>
    );
  },
};
</script>
