# Что такое XSS-уязвимость и как тестировщику не пропустить ее!

По моему наблюдению довольно много тестировщиков когда-либо слышали такое понятие, как XSS-уязвимость. Но мало кто может просто и на пальцах рассказать на собеседовании про нее. Или эффективно проверить веб-сайт на наличие этой уязвимости. Давайте вместе разберемся со всем этим подробнее и попробуем сами найти несложную XSS-уязвимость на демо-странице, которую я специально подготовил к этой статье.

Если вы гуру тестирования безопасности и на раз-два участвуете в баунти-программах крупных IT-компаний, а количество найденных вами XSS исчисляется десятками или даже сотнями — можно смело проходить мимо этой статьи. Если же вы новичок в теме и только начинаете интересоваться поиском уязвимостей — добро пожаловать под кат.

<script>alert(123)</script>

![img](./script.jpeg)

ля ля ля 