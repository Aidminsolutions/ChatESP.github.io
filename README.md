<head>
  <title>Botpress in a div</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      display: flex;
      justify-content: center;
      align-items: center;
      height: 100vh;
      margin: 0;
      color: white;
      background-color: #000000;
      font-family: Arial, sans-serif;
    }

    .center-div {
      width: 100vw;
      height: 100vh;
      background-color: rgb(0, 0, 0);
      border-radius: 0px;
      padding: 0px;
      box-sizing: border-box;
      color: white;
      display: flex;
      justify-content: center;
      align-items: center;
      text-align: center;
    }

    @media only screen and (max-width: 600px) {
      .center-div {
        height: 40vh;
        width: 80vw;
        background-color: rgb(102, 71, 255);
        border-radius: 0px;
        padding: 5px;
        box-sizing: border-box;
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        text-align: center;
      }
    }
  </style>
</head>

<body>
  <div> 
    
    <div class="absolute inset-4 ">
      <div class="center-div rounded-md border-zinc-200 bg-white p-2 relative h-full w-full overflow-clip border px-0 py-0">
        <iframe style="border: none;" srcdoc="<body><script src='https://cdn.botpress.cloud/webchat/v0/inject.js'></script>
            <script>
              let pathName = window.parent.location.href //this is to define url as a variable
              window.botpressWebChat.init({
                  'composerPlaceholder': 'Start typing..',
                  'botConversationDescription': 'BOEM’s Environmental Studies Program’s AI Assistant',
                  'botId': '77c81394-f515-4c42-be8e-cdaf341c80de',
                  'hostUrl': 'https://cdn.botpress.cloud/webchat/v0',
                  'messagingUrl': 'https://messaging.botpress.cloud',
                  'clientId': '77c81394-f515-4c42-be8e-cdaf341c80de',
                  'enableConversationDeletion': true,
                  'botName': 'ChatESP',
                  'showPoweredBy': false,
                  'className': 'webchatIframe',
                  'containerWidth': '100%25',
                  'layoutWidth': '100%25',
                  'hideWidget': true,
                  'showCloseButton': false,
                  'disableAnimations': true,
                  'closeOnEscape': false,
                  'showConversationsButton': false,
                  'enableTranscriptDownload': false,
                  'stylesheet':'https://webchat-styler-css.botpress.app/prod/code/d2daf807-ec41-450c-b8f7-50a3dc117758/v30179/style.css',
                  'userData': {
                  'path': pathName} //this is to pass URL into the bot
                  
              });
            window.botpressWebChat.onEvent(function () { window.botpressWebChat.sendEvent({ type: 'show' }) }, ['LIFECYCLE.LOADED']);
            </script></body>" width="100%" height="100%"></iframe>
      </div>
    </div>
  </div>
</body>
</html>
# ChatESP.github.io
