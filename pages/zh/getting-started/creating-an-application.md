# 创建一个应用

在这一节中，你会了解到我们在上一节中创建的项目各个文件的含义。

如果你不想了解这么多，你可以直接跳过这一节。

## 入口点文件

对于 Vercel 来说，它需要一个导出的函数。

```TypeScript
module.exports = async function(request:VercelRequest, response:VercelResponse) {};
```

在这个函数里面，我们可以编写我们的主体代码。

### 主函数

首先，我们需要创建一个新的 **应用实例**。

```TypeScript
const app = new VCLight();
```

接下来的部分中，你可以使用`app.use(middleware)`来应用中间件实例。

::: tip

我们不建议你在这个部分编写你的主体代码。

在接下来的教程中，主体代码会在`src/app/` 底下。
:::
