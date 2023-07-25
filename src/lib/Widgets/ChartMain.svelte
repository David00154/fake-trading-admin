<script>
  import { onMount } from "svelte";

  onMount(() => {
    // @ts-ignore
    new TradingView.widget({
      width: "100%",
      height: 550,
      symbol: "BITSTAMP:BTCUSD",
      interval: "D",
      timezone: "Etc/UTC",
      theme: "dark",
      style: "1",
      locale: "en",
      toolbar_bg: "#f1f3f6",
      enable_publishing: false,
      withdateranges: true,
      hide_side_toolbar: false,
      allow_symbol_change: true,
      show_popup_button: true,
      popup_width: "1000",
      popup_height: "650",
      container_id: "tradingview_e8033",
    });
  });
</script>

<div class="main-chart mb15 dark-variant">
  <!-- TradingView Widget BEGIN -->
  <div class="tradingview-widget-container">
    <div id="tradingview_e8033" />
  </div>
  <!-- TradingView Widget END -->
</div>
