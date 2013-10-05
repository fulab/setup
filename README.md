# Requirements

ansible

# Example

以下のようなインベントリファイルを作る
```
[isucon]
test ansible_ssh_host=<hostname> ansible_ssh_user=ec2-user
```

そのファイルを -i オプションで指定する
```
$ ansible-playbook -v -i hosts basic.yml --private-key=<path_to_private_key>
```
