# BOOTSTRA.386 for ASP.NET MVC

Base on [BOOTSTRA.386](https://github.com/kristopolous/BOOTSTRA.386) with tiny modify.  
**Not Bootstrap 4**

![demo img](https://i.imgur.com/5bfLA7c.gif)

### Usage  
Assume your MVC project theme didn't modify before, just replace/add following folder to project.
```
Content
fonts
Scripts
```
Then add bootstrap-386.js in `App_Start\BundleConfig.cs`.
```
bundles.Add(new ScriptBundle("~/bundles/bootstrap").Include(
            "~/Scripts/bootstrap.js",
            "~/Scripts/bootstrap-386.js"));
```
If need, add js setting in `Views\Shared\_Layout.cshtml` or other place you like to.
```
<script>
    _386 = { onePass: true, speedFactor: 1.5 };
</script>
``` 
That's all.