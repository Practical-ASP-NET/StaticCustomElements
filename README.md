# Blazor Custom Elements Demo

This repo demonstrates using Blazor's new (in .NET 7) custom element support in Blazor WASM sites that are deployed statically.

## Publish (for deployment to static site)

``` powershell
dotnet publish -c Release -o release
```

Copy the resulting release/wwwroot folder to your static site provider and you should be good to go.

Note, depending on your provider you may need to add extra config to redirect all requests to index.html. 

Check the wwwroot folder for netlify.toml which does this for Netlify.

Check out the (very impressive, don't you think) running version of this app here: https://visionary-zabaione-eec24a.netlify.app/
