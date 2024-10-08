# Тестовое задание на тему "Детекция и трекинг футбольного мяча" 

## Датасет
[Датасет SoccerNet](https://github.com/SoccerNet/sn-gamestate?tab=readme-ov-file#manual-downloading-of-soccernet-gamestate)

## Готовые модели
[Готовые модели](https://drive.google.com/drive/folders/1OjVZOkpxtzomTt7k5JNHmKylUlr5-jPO?usp=sharing)

## Финальные обработанные видео
[Видео](https://drive.google.com/drive/folders/1D29nDXVii0QpQhrRS-EG_Tt2sgi5dCuO?usp=sharing)

## Инструкция по запуску
В ходе работы был создан Jupyter Book. Чтобы полностью протестировать его и получить предсказания на видео, стоит просто запускать его по пунктам, обращая внимание на некоторые дополнения в заголовках. Для детекции и трекинга использовалась библиотека **Detectron2**. 

## Основная модель
- **Итерации:** 5000
- **Классы:** 5 (player, referee, goalkeeper, ball, other)

## Дополнительные модели
1. **Модель 1**
   - **Итерации:** 5000
   - **Классы:** 1 (ball)
   - **Использование:** С использованием предобученной model zoo
   - **Результаты:** На видео видны улучшения по сравнению с предыдущей моделью, но все также плохо. [Видео](https://drive.google.com/file/d/1vdDZ0nb4JNEe2wyST9ECyJHy1kf91hbS/view?usp=sharing)

2. **Модель 2**
   - **Итерации:** 5000
   - **Классы:** 1 (ball)
   - **Использование:** БЕЗ использования предобученной model zoo
   - **Результаты:** По итогу дает плохие результаты на challenge части. [Видео](https://drive.google.com/file/d/179wfqIl0lAUncoOvKeg9Bu4XLtCHyQeR/view?usp=sharing)
