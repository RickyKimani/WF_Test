
  <head>
    <meta charset="utf-8" />
    <title>Web Flash Webpage</title>
    <style>
      body {
        font-family: -apple-system, system-ui, BlinkMacSystemFont, "Segoe UI",
          Roboto, Ubuntu, sans-serif;
        padding: 0;
        margin: 0;
        line-height: 1.4;
      }
      .content {
        max-width: 600px;
        margin: 0 auto;
        padding: 12px;
      }
      h2 {
        margin-top: 2em;
      }
      h3 {
        margin-top: 1.5em;
      }
      .projects {
        display: flex;
        text-align: center;
        flex-wrap: wrap;
        gap: 24px;
        justify-content: center;
      }
      .projects a {
        color: initial;
        text-decoration: none;
      }
      .project .logo img {
        height: 50px;
      }
      .project .name {
        margin-top: 8px;
      }
      a {
        color: #03a9f4;
      }
      .screenshot {
        text-align: center;
      }
      .screenshot img {
        max-width: 100%;
        box-shadow:
          rgb(0 0 0 / 20%) 0px 2px 1px -1px,
          rgb(0 0 0 / 14%) 0px 1px 1px 0px,
          rgb(0 0 0 / 12%) 0px 1px 3px 0px;
        border-radius: 4px;
      }
      .screenshot i {
        margin-top: 4px;
        display: block;
      }
      .videoWrapper {
        position: relative;
        padding-bottom: 56.25%; /* 16:9 */
        height: 0;
        margin-bottom: 25px;
        background: #ccc;
      }
      .hidden {
        display: none;
      }
      .content pre {
        display: block;
        padding-left: 8px;
        overflow-y: scroll;
      }
      .footer {
        margin-top: 24px;
        border-top: 1px solid #ccc;
        padding-top: 24px;
        text-align: center;
      }
      .footer .initiative {
        font-style: italic;
        margin-top: 16px;
      }
      table {
        border-spacing: 0;
      }
      td {
        padding: 8px;
        border-bottom: 1px solid #ccc;
      }
      @media (prefers-color-scheme: dark) {
        body {
          background-color: #333;
          color: #fff;
        }
        a {
          color: #58a6ff;
        }
      }
    </style>
    <script
      type="module"
      src="https://unpkg.com/esp-web-tools@3.4.2/dist/web/install-button.js?module"
    ></script>
  </head>
  <body>
    <div class="content">
      <h1>ESP Web Tools</h1>
      

      <esp-web-install-button
        manifest="test/manifest.json"
      >
        <i slot="unsupported">
          The demo is not available because your browser does not support Web
          Serial. Open this page in Google Chrome or Microsoft Edge instead<span
            class="not-supported-i hidden"
          >
            (but not on your iOS device)</span
          >.
        </i>
      </esp-web-install-button>
