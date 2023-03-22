# Отток клиентов

Предоставлены исторические данные о поведении клиентов и расторжении договоров с банком. 

Цель: спрогнозировать, уйдёт клиент из банка в ближайшее время или нет.  Для этого необходимо построить модель с предельно большим значением *F1*-меры. Нужно довести метрику до 0.59 на тестовой выборке.

В данном проекте мы решаем задачу классификации с помощью машинного обучения с учителем



Источник данных: [https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling](https://www.kaggle.com/barelydedicated/bank-customer-churn-modeling)

<h1>Содержание<span class="tocSkip"></span></h1>
<div class="toc"><ul class="toc-item"><li><span><a href="#Подготовка-данных" data-toc-modified-id="Подготовка-данных-1"><span class="toc-item-num">1&nbsp;&nbsp;</span>Подготовка данных</a></span><ul class="toc-item"><li><span><a href="#Изучение-и-предобработка-данных" data-toc-modified-id="Изучение-и-предобработка-данных-1.1"><span class="toc-item-num">1.1&nbsp;&nbsp;</span>Изучение и предобработка данных</a></span></li><li><span><a href="#Кодирование,-разделение-на-выборки-данных" data-toc-modified-id="Кодирование,-разделение-на-выборки-данных-1.2"><span class="toc-item-num">1.2&nbsp;&nbsp;</span>Кодирование, разделение на выборки данных</a></span></li><li><span><a href="#Масштабирование-признаков" data-toc-modified-id="Масштабирование-признаков-1.3"><span class="toc-item-num">1.3&nbsp;&nbsp;</span>Масштабирование признаков</a></span></li></ul></li><li><span><a href="#Исследование-задачи" data-toc-modified-id="Исследование-задачи-2"><span class="toc-item-num">2&nbsp;&nbsp;</span>Исследование задачи</a></span></li><li><span><a href="#Борьба-с-дисбалансом" data-toc-modified-id="Борьба-с-дисбалансом-3"><span class="toc-item-num">3&nbsp;&nbsp;</span>Борьба с дисбалансом</a></span><ul class="toc-item"><li><span><a href="#С-помощью-взвешивания-классов" data-toc-modified-id="С-помощью-взвешивания-классов-3.1"><span class="toc-item-num">3.1&nbsp;&nbsp;</span>С помощью взвешивания классов</a></span></li><li><span><a href="#С-помощью-увеличения-выборки" data-toc-modified-id="С-помощью-увеличения-выборки-3.2"><span class="toc-item-num">3.2&nbsp;&nbsp;</span>С помощью увеличения выборки</a></span></li><li><span><a href="#С-помощью-уменьшения-выборки" data-toc-modified-id="С-помощью-уменьшения-выборки-3.3"><span class="toc-item-num">3.3&nbsp;&nbsp;</span>С помощью уменьшения выборки</a></span></li></ul></li><li><span><a href="#Тестирование-модели" data-toc-modified-id="Тестирование-модели-4"><span class="toc-item-num">4&nbsp;&nbsp;</span>Тестирование модели</a></span></li><li><span><a href="#Чек-лист-готовности-проекта" data-toc-modified-id="Чек-лист-готовности-проекта-5"><span class="toc-item-num">5&nbsp;&nbsp;</span>Чек-лист готовности проекта</a></span></li></ul></div>

### Используемые библиотеки

pandas

scikit-learn