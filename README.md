# Лабораторна робота №5
## Мета: Навчитися пряцювати з react-router-dom

Дана робота є продовженням попередньої

1. Створити у склонованій директорії [React проект](https://vitejs.dev/guide/#scaffolding-your-first-vite-project) з назвою 'traffic-lights-5'
1. Перенести попередню лабораторну 
1. В папці src створити папку "Pages", а в ній компоненту "Home", на якій буде висвітлюватися завдання лабораторної роботи
2. В цій же папці стоврити компоненту "ErrorPage" реалізувавши в ній кастомний вивід інформації про помилку
1. Cтворити компоненту "Header", в якій реалізувати меню(меню має містити два пункти "Горизонтальний сфітлофор" та "Вертикальний світлофор") 
1. В App додати компоненту "Header"
1.  Підключти бібліотеку "react-roter-dom"; в "App" реалізувати наступні роути
    ```js
    const router = createBrowserRouter([
          {
            path: "/",
            element: <Home />,
            errorElement: <ErrorPage />
          },
            {
            path: "/horisontal",
            element: <... />,
            errorElement: <ErrorPage />
          },
            {
            path: "/vertikal",
            element: <... />,
            errorElement: <ErrorPage />
          },
        ]);

    ```
    * отримаєте незабутні враження, якщо  реалізуєте роути наступним чином
    ```js
    const router = createBrowserRouter([
          {
            path: "/",
            element: <Home />,
            errorElement: <ErrorPage />,
            childrean: [
            {
                path: ":direction",
                element: <... />
            }
                ]
          },
     ]);
    ``` 
1. Оформити звіт на локальному комп'ютері
1. Запушити лаборатону в github.classroom
1. В Google classroom додати посилання на звіт
