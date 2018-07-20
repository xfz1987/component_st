# router原理
## history
```
<a class="api a">a.html</a>
<a class="api b">b.html</a>
<script>
  // 注册路由
  document.querySelectorAll('.api').forEach(item => {
    item.addEventListener('click', e => {
      e.preventDefault()
      let link = item.textContent
      window.history.pushState({name: 'api'}, link, link)
    }, false)
  })
  // 监听路由
  window.addEventListener('popstate', e => {
    console.log({
      location: location.href,
      state: e.state
    })
  },false)
</script>
```

## hash
```
<a class="hash a">#a.html</a>
<a class="hash b">#b.html</a>
<script>
  // 注册路由
  document.querySelectorAll('.hash').forEach(item => {
    item.addEventListener('click', e => {
      e.preventDefault()
      let link = item.textContent
      location.hash = link
    }, false)
  })
  // 监听路由
  window.addEventListener('hashchange', e => {
    console.log({
      location: location.href,
      hash: location.hash
    })
  },false)
</script>
```