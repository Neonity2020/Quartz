## 标题

## 标题2

```
## 标题2
```
### 标题3

```
### 标题3
```

## 代码块

```Typescript
export default async function Page() {
  const data = await fetch('https://api.vercel.app/blog')
  const posts = await data.json()
  return (
    <ul>
      {posts.map((post) => (
        <li key={post.id}>{post.title}</li>
      ))}
    </ul>
  )
}
```

## 公式块

$$

E = mc^{2}

$$
## 参考链接

- [PKMer.cn Markdown for OB](https://pkmer.cn/Pkmer-Docs/02-%E7%9F%A5%E8%AF%86%E7%AE%A1%E7%90%86%E5%9F%BA%E7%A1%80/markdown/markdown%E8%B6%85%E7%BA%A7%E6%95%99%E7%A8%8B-obsidian%E7%89%88/)

