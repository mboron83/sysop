###Restart ferm@docker

```
ip netns exec __NAMESPACE__ ferm -F /etc/ferm/docker/__CFG_FILENAME__.ferm && \
ip netns exec __NAMESPACE__ ferm /etc/ferm/docker/__CFG_FILENAME__.ferm
```
