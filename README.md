#### Создание токена и его авторизация в бэкофисе
- Для начала необходимо создать свой приватный токен доступа. Он необходим, чтобы статьи можно было добавлять из любого репозитория, к которому у вас есть доступ. Для этого кликаем на аватарку своего профиля и переходим в 'Settings'

![image](https://user-images.githubusercontent.com/48432436/169388472-a0d2ad9c-121b-4735-ad81-f8ccdc644d9e.png)

- В появившемся окне листаем в самый низ и переходим по самой последней вкладке 'Developer settings'. Далее 'Personal access token'(Третья по счету и последняя) и 'Generate new token' 

- Заполняем название токена (Оно больше не пригодится) и выдаем следующие права:

![image](https://user-images.githubusercontent.com/48432436/169390199-6e6cc6cb-c281-44d3-b217-fccaff61b6a5.png)

- Кликаем на 'Generate token' в самом низу странице. После успешного сохранения вы увидите текст токена. Его необходимо записать, второго шанса не будет

![token](https://user-images.githubusercontent.com/48432436/169391439-cecbc699-1c95-4036-90f9-840aa52976cf.png)


[TODO: БУДЕТ ИСПРАВЛЕНО ПОСЛЕ ФУНКЦИОНАЛА В БЭКОФИСЕ] 
- Переходим в плейгранд, проходим авторизацию и получаем accessToken
```
signIn(data: { login: "Логин", password: "Пароль" }){
    tokens{
      accessToken
    }
```

- Далее необходимо привязать учетную запись бэкофиса, персональный токен и аккаунт на гитхабе. Для этого accessToken из предыдущего запрос проставляем в качестве 'authorization-token'

```
 setGithubPrivateToken(data: {
    token: "Здесь должен быть токен, который был сгенерирован ранее",
    githubLogin: "Логин гитхаба"
```

#### Добавление постов

- Возможно только после создания приватного токена и его авторизации

- Создать отдельную ветку от main, в текстовом поле ввести название новой ветки, нажать на Create branch
 
![pr_creating](https://user-images.githubusercontent.com/48432436/165773036-c069375a-be64-4acc-9588-f7feff17f86d.png)

- Перейти в новую ветку и кликнуть 'Add file' => 'Upload files'

![file_upload](https://user-images.githubusercontent.com/48432436/165773878-ec09aa84-1e31-4bd3-9f5d-75bfa10ed0b5.png)

- Перетащить файл поста или папку с файлом в поле на новой странице. После успешной загрузки нажать зеленую кнопку 'Commit changes'
  - При создании нового поста важно убедиться, что папка с таким именем не существует в основной ветке, иначе существующий пост будет обновлен ( за раз можно добавить не более 30 файлов)

![drag_n_drop](https://user-images.githubusercontent.com/48432436/165774478-9143844f-141a-4fda-8602-2b4c183768dc.png)

- Если все прошло успешно, то на экране появится соответствующее сообщение, в котором предлагается создать Pull Request. Кликаем зеленую кнопку 'Compare & pull request'

![create_pr](https://user-images.githubusercontent.com/48432436/165775602-7d316595-dc96-455a-8b18-aa0ca94afc08.PNG)

- В новом окне надо задать информацию о Pull Request. Поля заголовка и описания используются только для удобства редактора, они не играют абсолютно никакой роли в формировании поста. Те лейблы, которые будут проставлены в поле 'labels' в дальнейшем станут тегами поста. На данном этапе необязательно заполнять все как в последний раз, у вас еще будет возможно все отредактировать. После всех приготовлений кликаем зеленую кнопку 'Create pull request'

![Pr_desc](https://user-images.githubusercontent.com/48432436/165777031-a5195bf2-cd7a-465d-a010-487b23bc444d.PNG)

- В следующем окне отображается вся информация о вашем Pull Request, вы в любой момент можете его закрыть и вернуться позднее, прогресс не пропадет. Создание поста происходит после клика на кнопку 'Merge pull request'


#### Обновление существующего поста
- Если вам надо обновить только теги, то можно использовать Pull Request, который создавался ранее для создания поста, в случае изменения тегов в этом PR они автоматически изменятся в посте. Для редактирования остальных полей необходимо пройти процедуру создания поста снова. При обновлении поста важно учитывать его расположение в основной ветке проекта. То есть, если файл поста, который вы хотите изменить, называется 'PostAboutForest.md' и находится в папке 'Forest', то в новой ветке он так же должен находится в папке 'Forest' и иметь названия 'PostAboutForest.md'. Остальные полностью действия аналогичны созданию поста

#### Варианты размещения заголовка, описания, превью в статье
- Заголовок
  - Первая строка в файле, обязательно наличие '#' перед заголовком
  - Рядом (На соседних строках) с превью
  - Если предыдущие 2 пункта не выполнены, то первые 4 слова описания
- Описание
  - Первый абзац в статье (!! При отсутствии разделения текста на абзацы в описании весь текст статьи)
- Превью
  - Первая картинка (.jpg, .png, .jpeg) в статье
  - Если превью не на соседних строках с описанием или заголовком, то пустая строка

#### Ограничения по количеству символов в посте
- Заголовок 180 символов
- Описание 100000 символов
- Контент 100000 символов

#### Рекомендации к изображениям
- Желателен любой горизонтальный формат. Соотношение сторон между 4:3 и 16:9 либо приближенное .
