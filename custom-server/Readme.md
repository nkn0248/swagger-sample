# custom-server

cf : https://github.com/go-swagger/go-swagger/tree/43c2774170504d87b104e3e4d68626aac2cd447d/examples/tutorials/custom-server
cf : https://goswagger.io/tutorial/custom-server.html

## 初回実行
1. swaggerファイル作成
2. swagger generate server -t gen -f ./swagger/swagger.yml --exclude-main -A greeter
    2.1 main.goは編集したいので、自動生成からは除外
3. ./cmd/greeter/main.goを作成。（公式githubを参照）
4. `go run ./cmd/greeter/main.go --port 3000`
5. curl