# Аппликативные модели для предсказания вероятности дефолта по кредитам
### Постановка задачи

**О компании**  
Компания Х специализируется на предоставлении частных кредитов. Клиенты подают заявки на кредиты, после чего компания проверяет их данные на соответствие критериям получения финансирования.

**Задача**  
Компания X стремится автоматизировать процесс оценки права клиента на получение кредита в режиме реального времени, используя данные, предоставленные клиентами в онлайн-заявках. 
Для достижения этой цели нами было обучено несколько предсказательных моделей, популярных в банковской сфере — специально для оценки вероятности списания долга.

### Описание проекта

В рамках данного проекта были выполнены следующие шаги:

- **Анализ набора данных:**
  - Изучены данные о клиентах, включая такие характеристики, как цель кредита, опыт работы, ежемесячный доход и кредитная история.
  - Проведен анализ общей информации для понимания структуры данных и выявления потенциальных проблем с качеством данных.
  
- **Предобработка данных:**
  - Обработаны шум и экстремальные значения, а также исправлены отрицательные и отсутствующие значения.
  - Различные единицы измерения были преобразованы для обеспечения корректного сравнения (например, ежемесячные расходы были переведены в годовые).
  - Выявлены выбросы и заменены на вероятные средние значения.

- **Статистический анализ переменных:**
  - Осуществлен анализ нормальности распределения, количественных и категориальных переменных.
  - Применены логарифмические преобразования для сглаживания распределений данных.
  
- **Анализ взаимосвязей:**
  - Проведен анализ с двумя переменными для выявления сильных категориальных факторов, корреляций и осуществлена проверка статистической значимости числовых переменных относительно целевой переменной (статус платежа).

- **Преобразование категориальных признаков:**
  - Категориальные признаки были обработаны для корректного использования в моделях, и подготовлены тренировочная и тестовая выборки.
  - Масштабированы данные для улучшения производительности моделей методом Target Encoding.

- **Моделирование:**
  - Обучены следующие аппликативные модели для задачи бинарной классификации:
    - Логистическая регрессия
    - Gradient Boosting
    - XGBoost
    - Метод опорных векторов (SVM)
    - Дерево решений
    - Случайный лес (Random Forest)
  - Для каждой модели была выполнена настройка гиперпараметров, обучение и последующая оценка производительности с использованием метрик, таких как коэффициент Джини и другие показатели качества.

- **Общий вывод и рекомендации:**
  - Проанализированы полученные результаты, выделены сильные факторы, влияющие на вероятность невыплаты кредита.
  - Предоставлены рекомендации для улучшения процесса одобрения кредитов на основе предоставленных моделей.

### Используемые технологии
- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib/Seaborn