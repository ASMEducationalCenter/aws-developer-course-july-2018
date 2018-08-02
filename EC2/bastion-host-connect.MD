### Start the ssh agent:
```
eval `ssh-agent -s`
```


enter this command to add the key to the agent:


```
$ssh-add  yourkey.pem
```

You should see an output of “Identity added”

Now when you ssh into the Bastion Host, instead of the -i just do this:
```
$ ssh -A user@IPADRESS
```

Once you're inside the public instance ssh into the private Instance using the private ip
```
ssh ec2-user@10.11.12.13
```
