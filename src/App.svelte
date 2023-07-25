<script>
  import Header from "./lib/Header.svelte";
  import BuySellBox from "./lib/Widgets/BuySellBox.svelte";
  import ChartMain from "./lib/Widgets/ChartMain.svelte";
  import OrderBook from "./lib/Widgets/OrderBook.svelte";
  import PairSelector from "./lib/Widgets/PairSelector.svelte";
  import RecentTrades from "./lib/Widgets/RecentTrades.svelte";
</script>

<Header />
<div class="container-fluid mtb15 no-fluid">
  <div class="row sm-gutters">
    <div class="col-md-3">
      <PairSelector />
    </div>
    <div class="col-md-9">
      <div class="row sm-gutters">
        <div class="col-12">
          <ChartMain />
        </div>
        <div class="col-md-8">
          <BuySellBox />
        </div>
        <div class="col-md-4">
          <OrderBook />
        </div>
      </div>
    </div>
  </div>
</div>
