# gRPC PHP Client Library

This repository contains only PHP files to support Composer installation.

This repository is a mirror of [gRPC](https://github.com/grpc/grpc). Any support
requests, bug reports, or development contributions should be directed to
that project.

To install gRPC for PHP, please see https://github.com/grpc/grpc/tree/master/src/php

for plaintext request

`php $channel = new \Grpc\Channel('0.0.0.0:50051',[]); $client = new Helloworld\GreeterClient(null, null, $channel); $request = new Helloworld\HelloRequest(); $request->setName($name); list($reply, $status) = $client->SayHello($request)->wait(); $message = $reply->getMessage();`
