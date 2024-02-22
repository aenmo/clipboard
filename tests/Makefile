# Copyright 2021 The golang.design Initiative Authors.
# All rights reserved. Use of this source code is governed
# by a MIT license that can be found in the LICENSE file.
#
# Written by Changkun Ou <changkun.de>

all: test

test:
	go test -v -count=1 -covermode=atomic ..

test-docker:
	docker build -t github.com/aenmo/clipboard ..
	docker run --rm --name cb github.com/aenmo/clipboard
	docker rmi github.com/aenmo/clipboard