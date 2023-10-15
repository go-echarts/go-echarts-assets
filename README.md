# go-echarts-assets

go-echarts-assets is the turn key solution for hosting go-echarts javascript assets.  
It can be placed as it is into your server and its gh-pages acts as the default content delivery host when you evaluate go-echarts for web purposes.
i.e.

On page usage
```go
        page := components.NewPage()
	page.AssetsHost = "https://cdn.jsdelivr.net/npm/echarts@5.4.3/dist/"
```

On single chart usage
```go
	bar := charts.NewBar()
	bar.SetGlobalOptions(
		charts.WithInitializationOpts(opts.Initialization{
			AssetsHost: "https://cdn.jsdelivr.net/npm/echarts@5.4.3/dist/",
		}),
        )

```