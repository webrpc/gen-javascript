.PHONY: all generate diff

all: generate diff

generate:
	webrpc-gen -schema=./hello-webrpc/hello-api.ridl -target=../ -extra=noexports -client -out=./hello-webrpc/webapp/client.gen.js

diff:
	git diff --color --ignore-all-space --ignore-blank-lines --exit-code .
