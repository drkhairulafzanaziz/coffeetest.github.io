# Welcome to your Dyad app
<div id="coffee-survey-iframe-5hc15a4cd-container" style="width: 100%;">
  <iframe
    id="coffee-survey-iframe-5hc15a4cd"
    src="https://68sskvo8f4w74q31idpp2h3z0vleu6g5qoonykr23js01gwmmd-h791210728.scf.usercontent.googhttps://68sskvo8f4w74q31idpp2h3z0vleu6g5qoonykr23js01gwmmd-h791210728.scf.usercontent.goog/0bd4fb79-9566-4bf5-ae8e-2e6d532162af?embed=true"
    frameborder="0"
    scrolling="no"
    style="width: 1px; min-width: 100%; border: 1px solid #ccc; border-radius: 12px;"
    title="Coffee Cupping Survey Form"
  ></iframe>
</div>
<script>
(function() {
  var iframe = document.getElementById('coffee-survey-iframe-5hc15a4cd');
  if (!iframe) { return; }
  
  // Set an initial height to prevent layout shift while the form loads
  iframe.height = '1250px';

  var lastHeight = 0;
  var RESIZE_MESSAGE_TYPE = 'coffee-survey-resize';

  window.addEventListener('message', function(event) {
    // For production, you can strengthen security by checking event.origin
    if (
      event.data &&
      typeof event.data === 'object' &&
      event.data.type === RESIZE_MESSAGE_TYPE &&
      typeof event.data.height === 'number' &&
      event.source === iframe.contentWindow
    ) {
      var newHeight = event.data.height;
      if (newHeight !== lastHeight) {
        // Add a small buffer to prevent scrollbars from appearing on some browsers
        iframe.style.height = (newHeight + 16) + 'px';
        lastHeight = newHeight;
      }
    }
  });
})();
</script>
