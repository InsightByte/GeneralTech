### Install
```brew install chruby ruby-install```


### Configure Shell
```
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.1" >> ~/.zshrc
```

### S3 policy
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::<yout bucket name>/*"
        }
    ]
}
```
### Copy to S3 bucket
```
cd <path to your blog>
aws s3 sync _site s3://yout bucket name>/ --delete
```



