# Zadanie 1. Galeria obrazów

Wykonaj to zadanie w plikach 01-gallery.html i 01-gallery.js.

W poprzednim zadaniu domowym utworzyłeś/aś galerię obrazów przy użyciu delegowania zdarzeń i dodałeś/aś okno modalne za pośrednictwem biblioteki CDN, aby wyświetlać pełnowymiarową wersję obrazu.

Tworzenie galerii jest codziennym zadaniem dla programistów, ale ręczne pisanie ich za każdym razem jest zbyt czasochłonne. W tym celu istnieją biblioteki, które implementują całą logikę galerii.

Utwórz tę samą galerię, ale przy użyciu biblioteki SimpleLightbox, która zajmie się kliknięciami obrazów, otwieraniem i zamykaniem okna modalnego oraz przewijaniem obrazów za pomocą klawiatury.


Zwróć uwagę na następujące niuanse:

* Nie trzeba już wdrażać delegowania zdarzeń, biblioteka SimpleLightbox sama będzie śledzić kliknięcia na kartach galerii.
* Nie potrzebujesz już biblioteki do tworzenia okna modalnego, ta funkcjonalność jest wbudowana w bibliotece SimpleLightbox.

Wykonaj to zadanie w plikach gallery.html i gallery.js. Podziel to zadanie na kilka podzadań.



Użyj kodu z poprzedniego zadania domowego i dokonaj jego refaktoryzacji. Nie musisz pisać wszystkiego od nowa. Na przykład, tworzenie elementów galerii pozostanie bez zmian. Ale kod delegujący i otwierający okno modalne powinien zostać usunięty.

Dodaj bibliotekę SimpleLightbox jako zależność projektu za pomocą npm . Aby dołączyć kod CSS biblioteki do projektu, należy dodać kolejny import, oprócz tego opisanego w dokumentacji.

Następnym krokiem jest inicjalizacja biblioteki po utworzeniu i dodaniu elementów galerii do ul.gallery. Aby to zrobić, przeczytaj dokumentację SimpleLightbox, zwłaszcza sekcje „Usage” i „Markup”.

Następnie zapoznaj się z dokumentacją w sekcji „Opcje” i dodaj wyświetlane podpisy do obrazów z atrybutu alt. Niech podpis będzie na dole i pojawi się 250 milisekund po otwarciu okna modalnego.

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

# Zadanie 2. Formularz zwrotny

Wykonaj to zadanie w plikach 02-form.html i 02-form.js.

Dodaj do HTML znaczniki formularza. W JS napisz skrypt, który będzie zapisywał wartości pól w pamięci lokalnej, gdy użytkownik coś wpisze.


Wykonaj to zadanie w plikach feedback.html i feedback.js.

Podziel go na kilka podzadań:

1. Korzystając z delegowania, śledź zdarzenie input w formularzu i za każdym razem zapisuj obiekt z polami email i message do pamięci lokalnej, w której przechowywane są bieżące wartości pól formularza. Niech kluczem dla magazynu będzie ciąg „feedback-form-state”.
2. Po załadowaniu strony sprawdź stan pamięci, a jeśli są tam przechowywane dane, wypełnij nimi pola formularza. W przeciwnym razie pola powinny być puste.
3. Podczas submitu formularza wyczyść pamięć formularza i pola, a następnie wyświetl w konsoli obiekt z polami e-mail, message i ich aktualnymi wartościami.







# Vanilla App Template

Цей проект було створено за допомогою Vite. Для знайомства та налаштування
додаткових можливостей [звернись до документації](https://vitejs.dev/).

## Створення репозиторію за шаблоном

Використовуй цей репозиторій організації GoIT як шаблон для створення
репозиторію свого проекту. Для цього натисни на кнопку `«Use this template»` і
обери опцію `«Create a new repository»`, як показано на зображенні.

![Creating repo from a template step 1](./assets/template-step-1.png)

На наступному етапі відкриється сторінка створення нового репозиторію. Заповни
поле його імені, переконайся, що репозиторій публічний, після чого натисни
кнопку `«Create repository from template»`.

![Creating repo from a template step 2](./assets/template-step-2.png)

Після того, як репозиторій буде створено, необхідно перейти в налаштування
створеного репозиторію на вкладку `Settings` > `Actions` > `General` як показано
на зображенні.

![Settings GitHub Actions permissions step 1](./assets/gh-actions-perm-1.png)

Проскроливши сторінку до самого кінця, в секції `«Workflow permissions»` обери
опцію `«Read and write permissions»` і постав галочку в чекбоксі. Це необхідно
для автоматизації процесу деплою проекту.

![Settings GitHub Actions permissions step 2](./assets/gh-actions-perm-2.png)

Тепер у тебе є особистий репозиторій проекту, зі структурою файлів та папок
репозиторію-шаблону. Далі працюй з ним, як з будь-яким іншим особистим
репозиторієм, клонуй його собі на комп'ютер, пиши код, роби коміти та відправляй
їх на GitHub.

## Підготовка до роботи

1. Переконайся, що на комп'ютері встановлено LTS-версію Node.js.
   [Скачай та встанови](https://nodejs.org/en/) її якщо необхідно.
2. Встанови базові залежності проекту в терміналі командою `npm install`.
3. Запусти режим розробки, виконавши в терміналі команду `npm run dev`.
4. Перейдіть у браузері за адресою
   [http://localhost:5173](http://localhost:5173). Ця сторінка буде автоматично
   перезавантажуватись після збереження змін у файли проекту.

## Файли і папки

- Файли розмітки компонентів сторінки повинні лежати в папці `src/partials` та
  імпортуватись до файлу `index.html`. Наприклад, файл з розміткою хедера
  `header.html` створюємо у папці `partials` та імпортуємо в `index.html`.
- Файли стилів повинні лежати в папці `src/css` та імпортуватись до HTML-файлів
  сторінок. Наприклад, для `index.html` файл стилів називається `index.css`.
- Зображення додавай до папки `src/img`. Збирач оптимізує їх, але тільки при
  деплої продакшн версії проекту. Все це відбувається у хмарі, щоб не
  навантажувати твій комп'ютер, тому що на слабких компʼютерах це може зайняти
  багато часу.

## Деплой

Продакшн версія проекту буде автоматично збиратися та деплоїтись на GitHub
Pages, у гілку `gh-pages`, щоразу, коли оновлюється гілка `main`. Наприклад,
після прямого пуша або прийнятого пул-реквесту. Для цього необхідно у файлі
`package.json` змінити значення прапора `--base=/<REPO>/`, для команди `build`,
замінивши `<REPO>` на назву свого репозиторію, та відправити зміни на GitHub.

```json
"build": "vite build --base=/<REPO>/",
```

Далі необхідно зайти в налаштування GitHub-репозиторію (`Settings` > `Pages`) та
виставити роздачу продакшн версії файлів з папки `/root` гілки `gh-pages`, якщо
це не було зроблено автоматично.

![GitHub Pages settings](./assets/repo-settings.png)

### Статус деплою

Статус деплою крайнього коміту відображається іконкою біля його ідентифікатора.

- **Жовтий колір** - виконується збірка та деплой проекту.
- **Зелений колір** - деплой завершився успішно.
- **Червоний колір** - під час лінтингу, збірки чи деплою сталася помилка.

Більш детальну інформацію про статус можна переглянути натиснувши на іконку, і в
вікні, що випадає, перейти за посиланням `Details`.

![Deployment status](./assets/deploy-status.png)

### Жива сторінка

Через якийсь час, зазвичай кілька хвилин, живу сторінку можна буде подивитися за
адресою, вказаною на вкладці `Settings` > `Pages` в налаштуваннях репозиторію.
Наприклад, ось посилання на живу версію для цього репозиторію

[https://goitacademy.github.io/vanilla-app-template/](https://goitacademy.github.io/vanilla-app-template/).

Якщо відкриється порожня сторінка, переконайся, що у вкладці `Console` немає
помилок пов'язаних з неправильними шляхами до CSS та JS файлів проекту
(**404**). Швидше за все у тебе неправильне значення прапора `--base` для
команди `build` у файлі `package.json`.

## Як це працює

![How it works](./assets/how-it-works.png)

1. Після кожного пуша у гілку `main` GitHub-репозиторію, запускається
   спеціальний скрипт (GitHub Action) із файлу `.github/workflows/deploy.yml`.
2. Усі файли репозиторію копіюються на сервер, де проект ініціалізується та
   проходить лінтинг та збірку перед деплоєм.
3. Якщо всі кроки пройшли успішно, зібрана продакшн версія файлів проекту
   відправляється у гілку `gh-pages`. В іншому випадку, у лозі виконання скрипта
   буде вказано в чому проблема.
