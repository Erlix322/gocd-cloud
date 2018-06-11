# GoCD cloud images

Create GoCD server and agent images for docker, AWS, Azure...

#Building

```
$ packer build -var 'gocd_version=xx.x.x' go-server-packer.json
$ packer build -var 'gocd_version=xx.x.x' go-server-demo-packer.json
```

If the ec2 instance that is used to build the AMI needs to change, provide the `instance_type` variable as follows:

```
$ packer build -var 'gocd_version=xx.x.x' -var 'instance_type=c4.large' go-server-packer.json
$ packer build -var 'gocd_version=xx.x.x' -var 'instance_type=c4.large' go-server-demo-packer.json
```


# License

```plain
Copyright 2018 ThoughtWorks, Inc.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
