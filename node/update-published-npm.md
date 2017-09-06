### 公開NPMの更新手順

```bash
npm version patch
git tag # -> new git tag will to be created automatically
git push origin tags/<<created tag>>
npm publish
git push origin master
```
