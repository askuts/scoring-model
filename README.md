# scoring-model

Схематичное представление методологии исследования:
![image](https://github.com/user-attachments/assets/b8aa8516-ac03-4115-8a91-a11dfd2f1d03)

# Описание процесса и критериев отбора инновационных проектов для тестирования

Для апробации разработанной скоринговой модели была сформирована выборка из 212 инновационных финтех-проектов. Основными источниками данных послужили ведущие отраслевые базы *Crunchbase* и *PitchBook*, аккумулирующие детальную информацию о стартапах, инвестиционных сделках и технологических трендах в сфере финансовых технологий.

## Ключевые критерии отбора проектов в выборку

1. **Наличие исторических данных об успешности проекта.**

   Ключевым условием для включения проекта в выборку было наличие релевантного целевого события (успешное завершение деятельности в рамках приобретения либо дефолта/банкротства).

2. **Полнота и достоверность данных по выбранным предикторам.**

   Для обеспечения качества входных данных модели проекты с пропусками в значениях более 30% признаков исключались из рассмотрения. Приоритет отдавался проектам из баз Crunchbase и PitchBook, прошедших независимую верификацию. Также были рассмотрены данные о проектах из открытых источников (LinkedIn, Twitter и др.).

3. **Репрезентативность проектов для генеральной совокупности.**

   Использование метода стратифицированной случайной выборки позволило контролировать соответствие распределений проектов в сэмпле по таким параметрам, как технологический стек, страна базирования и бизнес-модель. Согласно исследованиям, учет этих факторов позволяет существенно повысить обобщающую способность прогнозных моделей машинного обучения в задачах венчурной аналитики (Krishna et al., 2016).

В итоге сформированная тестовая выборка включила в себя **212** инновационных финтех-проектов, 62% из которых имели патенты на ключевые технологии. Распределение проектов по целевому признаку – 37% успешных (выход на приобретение) и 62% неуспешных. В целом, собранный датасет достаточно репрезентативен для отражения структуры и динамики инновационных процессов в глобальной финтех-индустрии. Стратификация выборки и контроль качества данных позволяют рассчитывать на достоверность и обобщающую способность получаемых эмпирических результатов.

