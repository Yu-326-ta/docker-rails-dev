# docker-rails ð³

![ãã¼ã ç»é¢](images/rails-docker.webp)

## container

**web container**<br>
rails6.1.7

**db container**<br>
mysql8.0


## ç°å¢æ§ç¯æ¹æ³
Rails ã®ç°å¢ãæ§ç¯ããããã£ã¬ã¯ããªã§ `git clone` ãè¡ãããã©ã«ããä½æããã
docker compose.yml ãã¡ã¤ã«ããããã£ã¬ã¯ããªã§ä»¥ä¸ã®ã³ãã³ããé ã«æã¤

1. `docker-compose run web rails new . --force --database=mysql` ã³ãã³ãã§webã³ã³ããã«Railsã¤ã³ã¹ãã¼ã«
2. `docker-compose build` ã³ãã³ãã§ã¤ã¡ã¼ã¸ããã«ããç´ã
3. config/database.ymlãpassword: passwordãhost: dbã«å¤æ´
4. `docker-compose run web rails db:create` ã³ãã³ãã§dbã³ã³ããã«ãã¼ã¿ãã¼ã¹ä½æ
5. `docker-compose up -d` ã³ãã³ãã§ã³ã³ãããä½æ
6. localhost:3000ã«ã¢ã¯ã»ã¹
