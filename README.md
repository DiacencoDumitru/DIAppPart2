* Теперь не внедряем зависимости вручную как мы это делали до этого, а это мы доверили Spring'у с помощью `<constructor-arg ref="musicBean"/>` (Dependency Injection)
* Изначально когда Spring читает файл `applicationContext.xml` он создаёт бины начиная у нас от `musicBean` и затем он уже дошёл до нашего бина `musicPlayer` и внедрил этот бин musicBean таким образом совершив Dependency Injection
