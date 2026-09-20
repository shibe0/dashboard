# しべの当番表

`https://shibe0.github.io/dashboard/`

中身（`d.json`）は **AES-256-CBC で暗号化し、HMAC-SHA256 で封をして**あります。
開くには合言葉が要ります。合言葉はこのリポジトリには入っていません
（Mac の `~/.claude/dashboard/.passphrase`）。

- 元の1枚を組む: `~/.claude/dashboard/build.py`
- 暗号にして表紙をつける: `~/.claude/dashboard/site_build.py`
- 押し出す: `~/.claude/dashboard/push.sh`
- 5分ごとに回す係: `com.shibe.dashboard-push`（launchd）

この写しでは **聞く札のボタンと「代理で貼ってOK」は押せません**
（答えの置き場が Artifact 側にあるため）。押すほうは Claude の当番表を使ってください。
