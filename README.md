# Welcome to My GitBook

This is a test to see if the MightyIframeIntegration works.

<script src="https://unpkg.com/mightyiframeintegration@latest/dist/mightyIframeIntegration.js"></script>

<button id="learnButton">Learn More</button>

<script>
  document.addEventListener('DOMContentLoaded', function() {
    mightyIframeIntegration.authorizePackage();
    const initializeSidebar = () => {
      if (window.initSidebar) {
        window.initSidebar({
          selector: '#learnButton',
          partnerId: 'Magic_Ball',
          theme: 'dark'
        });
        window.initSidebar({
          selector: '#learnButton1',
          partnerId: 'Magic_Ball',
          theme: 'dark'
        });
         window.initSidebar({
          selector: '#learnButton2',
          partnerId: 'Magic_Ball',
          theme: 'dark'
        });
      }
    };
    initializeSidebar();
  });
</script>