# PHP-CS-Fixer docker image

## User
We are recommend to use the images as an shell alias to access via short-command. To use simply php-cs-fixer everywhere on CLI add this line to your ~/.zshrc, ~/.bashrc or ~/.profile.

```
alias php-cs-fixer='docker run --rm --tty --volume $PWD:/app jacquesndl/php-cs-fixer $*'
```

If you don't have set the alias, use this command to run the container:
```
docker run --rm --tty --volume /path/to/project:/app jacquesndl/php-cs-fixer [some arguments for PHP-CS-Fixer]
```

For example:
```
docker run --rm --tty --volume /path/to/project:/app jacquesndl/php-cs-fixer fix . --rules=@PSR1,@PSR2,@Symfony
```
