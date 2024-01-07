1. Какие основные преимущества Bootstrap?

- Сокращения времени, необходимого для создания макета сайта. Фреймворк предлагает достаточное количество шаблонов и готовых решений;
- Кросс-браузерность и адаптивность. Сайты, созданные с помощью Bootstrap, идентично отображаются на разных устройствах и в современных браузерах;
- Простота использования. Для работы с фреймворком потребуются элементарные навыки верстки;

2. Как сделать желтую кнопку с помощью Bootstrap?
   Задать class="btn btn-warning"

3. Каким кодом можно сделать такую сетку?

   !https://file.notion.so/f/f/f098cfa4-dc31-41b0-a467-db910d3cff90/c92145de-3f68-467a-982b-a03446074357/Untitled.png?id=24ecedf1-a384-4270-8a70-b64c151780cc&table=block&spaceId=f098cfa4-dc31-41b0-a467-db910d3cff90&expirationTimestamp=1704744000000&signature=U1S7Y2UOV24vL74GGR4XwZwJ2DXiHYXJxUCkmIxNBSM&downloadName=Untitled.png

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0" shrink-to-fit="no">
    <title>Bootstrap</title>
    <!-- Подключение CSS файла bootstrap 5 -->
    <link href="./bootstrap/bootstrap.min.css" rel="stylesheet" />
    <style>
        .title {
            min-height: 10vh;
        }

        .buy_box {
            min-height: 66vh;
        }

        .description {
            min-height: 10vh;
        }

        .related {
            min-height: 10vh;
        }
    </style>

</head>

<body>
    <div class="container p-2">
        <div class="row p-0 gap-2 align-self-center">
            <div class="col btn btn-primary btn-group-vertical align-items-center">gallery</div>
            <div class="col p-0">
                <div class="col-12 btn btn-primary mb-2 title">title</div>
                <div class="col-12 btn btn-primary btn-group-vertical align-items-center buy_box">buy box</div>
            </div>
            <div class="row p-0 m-0">
                <div class="col btn btn-primary description">description</div>
            </div>
            <div class="row  p-0 m-0">
                <div class="col btn btn-primary related">related</div>
            </div>
        </div>

        <!-- Подключение JS файла Bootstrap -->
        <script src="./assets/bootstrap/bootstrap.bundle.min.js"></script>

</body>

</html>

4. Каким компонентом Bootstrap можно задать такой элемент?
   Копмпонентом progress-bar
   !https://s3-us-west-2.amazonaws.com/secure.notion-static.com/100332d0-fcea-4f74-8070-52f051f57524/Untitled.png

      <div class="progress">
      <div class="progress-bar" role="progressbar" style="width: 25%;" aria-valuenow="25" aria-valuemin="0" aria-valuemax="100">25%</div>
         </div>

5. Как убрать поля между колонками?
   для row gap-0, либо p-0 m-0 для col

6. Как сделать навигацию на Bootstrap?
<ul class="nav">
  <li class="nav-item">
    <a class="nav-link active" aria-current="page" href="#">Active</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Link</a>
  </li>
  <li class="nav-item">
    <a class="nav-link" href="#">Link</a>
  </li>
  <li class="nav-item">
    <a class="nav-link disabled">Disabled</a>
  </li>
</ul>

7. Что такое колонка **auto-layout ?**
   Колонки auto-layout могут автоматически “расти” и “урезаться” по ширине в рамках 12 колонок.
   Например, в сетке из двух колонок col-3 заберет 3 колонки, а col заберет остальные 8 колонок.

8. Как сделать центрирование содержимого по горизонтали? А по вертикали?
   flex-row, flex-column

9. Как задать адаптивность для колонки шириной в 50%, чтобы при ширине экрана меньше 768px она становилась шириной на весь экран?
   col-md-12

10. Что произойдет, если колонок станет больше 12?
    перенесется на следующий ряд
11. Как задать иконку инстаграм через font awesome?
    <i class="fa fa-instagram" aria-hidden="true"></i>

12. Чем отличается container от container-fluid?
    .container-fluid непрерывно изменяет размер по мере изменения ширины окна / браузера на любую величину, никогда не оставляя дополнительного пустого пространства по бокам, в отличие от того, как это делает .container. (Отсюда и название: "текучий" в противоположность "цифровому", "дискретному", "фрагментированному" или "квантованному").
