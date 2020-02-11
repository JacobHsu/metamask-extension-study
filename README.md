# metamask-extension-study

[metamask-extension](https://github.com/MetaMask/metamask-extension)

manifest.json

```
  "browser_action": {
    "default_popup": "popup.html"
  },
```

app\popup.html

```
<script src="./ui.js" ></script>
```

app\scripts\ui.js

```
import launchMetaMaskUi from '../../ui'
```

ui\index.js
```
import Root from './app/pages'

render(<Root />, opts.container);
```


ui\app\pages\index.js

```
import Routes from './routes'
 <Routes/>
```

ui\app\pages\routes\index.js

```
import FirstTimeFlow from '../first-time-flow'
<Route path={INITIALIZE_ROUTE} component={FirstTimeFlow} />
```


ui\app\pages\first-time-flow\first-time-flow.component.js

```
import Welcome from './welcome'
<Route
  exact
  path={INITIALIZE_WELCOME_ROUTE}
  component={Welcome}
/>
```


ui\app\pages\first-time-flow\welcome\welcome.component.js

```
    return (
      <div className="welcome-page__wrapper">
        <div className="welcome-page">
          Mascot welcome
```



C:\research\metamask-extension\app\scripts\metamask-controller.js

