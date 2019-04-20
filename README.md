# mch-hackathon

## Useful OFFCHAIN APIs

### Ethereum Address もしくは UIDを使ってCryptoWorldにあるユーザー情報を取得する
`https://www.mycryptoheroes.net/experimental-api/proxy/mch/users/(address|uid)`

### Plusmeta APIを使ってアセット価値内容を登録する
`POST https://www.mycryptoheroes.net/experimental-api/plusmeta/heroes/(heroid)`

sample data
```json
{"iss": "0xd868711BD9a2C6F1548F5f4737f71DA67d821090",
 "metadata": {
     "sub": "my crypto derbies",
     "aud": [
	 "https://example.com/"
     ],
     "name": "deeeeep blue",
     "description": "すごい",
     "attributes": {
	 "hp": 100,
	 "speed": 100,
	 "skill": [
	     "dart", "sunny"
	 ],
	 "kind": "Mare"
     }
 }
}
```

### Plusmeta APIに登録された価値内容を参照する
`GET https://www.mycryptoheroes.net/experimental-api/plusmeta/heroes/(heroid)`
