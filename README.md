# A Mirror Blog

Write or your post as issues in the repository, it will display pure and beautiful as a website.

# Steps

1.Install Mirror as a global module

```sh
npm i -g Mirror
```

2.Initiate your blog

```sh
mkdir blog
mirror init blog
```

3.Generate a token for your blog

[Generate Tokens](https://github.com/settings/tokens)

You should check 「public_repo」 and 「user:email」, it is not dangerous, just to read your issues more times from github api.

4.Configure your blog

Modified the 「config.yml」 file in your blog directory, like my configuration below:

```sh
# site title
title: 进击的前端

# user name or organization name
user: ricosmall

# issue repository
repository: mirror

# multi-author
authors: rico

# token
# token should be separated by '#'
# initial token: d6dcb062ee56583e5b438fef8b9d11c925f3f1cf
# after token: d#6dcb062ee56583e5b438fef8b9d11c925f3f1cf
token: d#6dcb062ee56583e5b438fef8b9d11c925f3f1cf

# posts per page
perpage: 10


# advance config

# organization repository (?)
organization: false

# post order
# order by create time" or "update time"
# 'UPDATED_AT' or 'CREATED_AT'
order: 'UPDATED_AT'
```

5.Build your blog

```sh
mirror build
```

6.Push your blog to a new repository into `gh-pages` branch

```sh
git remote add origin git@github.com:ricosmall/mirror
git add .
git commit -m 'something'
git push origin master:gh-pages -u
```

7.Add new issues

8.You can visit your blog website now

9.Comment function is already here below issues

10.Have fun