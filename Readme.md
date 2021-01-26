## 修改版 支持 gorm

## 使用说明

配合 cute-angelia/mysql-protobuf 使用， 该工具能快速将 sql 生成 proto3

```
git clone git@github.com:cute-angelia/gogo-protobuf.git

cd gogo-protobuf/protoc-gen-gofast && go install

```


## 说明

虽然有 [protoc-gen-gorm](https://github.com/infobloxopen/protoc-gen-gorm) 这个插件， 但是配置很烦，需要修改每个 proto 文件

之前也魔改过一个[protobuf](https://github.com/cute-angelia/protobuf)

这次选型 gogo ，也是项目需要, 这次打算接入斗鱼的 jupiter， jupiter 使用的是 gogo-protobuf

jupiter 里面 gorm 用法还很原始， 需要自己定义 model， 这里直接集成到工具里面

几行代码能搞定的事情，就不去花大力气（兼容grpc和gorm）写插件了