# Работы по дисциплине «Методы машинного обучения»
Исполнитель: Голубев Илья Игоревич, группа ИУ5-24М, 2018–2019 учебный год.

Каждая работа расположена в своей папке и содержит как все необходимые материалы, так и отчёт по данной работе. Отчёты формируются из Jupyter-ноутбуков с помощью nbconvert, команда приведена в README.md каждой работы.

# Список работ
  Лабораторная работа №1 (отчёт).

# Подготовка Jupyter-ноутбука для формирования отчёта
Чтобы превратить Jupyter-ноутбук в красивый отчёт, следует сделать следующее:

Добавить следующие метаданные в ноутбук (Edit -> Edit Notebook Metadata в классическом интерфейсе, через плагин jupyterlab_nbmetadata в Jupyter Lab, или просто открыв ноутбук в текстовом редакторе):
{
  "authors": [
    {
      "name": "Лещев Артем Олегович"
    }
  ],
  "group": "ИУ5-24М",
  "lab_number": 1,
  "title": "Разведочный анализ данных. Исследование и визуализация данных"
}
Если хочется библиографию:
Сделать символическую ссылку в папке с ноутбуком на common/bib.bib.
Расставить в ноутбуке в Markdown-ячейках ссылки вида:
<cite data-cite="ue:lab1"></cite>
После этого можно превратить данный Jupyter-ноутбук в отчёт командой вида:

jupyter nbconvert --to pdf --template=../common/template.tplx eda_visualization.ipynb
Вместо pdf можно использовать ключевое слово latex, чтобы получить готовый для редактирования .tex-файл. После редактирования следует использовать команду xelatex для компиляции этого файла в PDF.

При необходимости, естественно, можно подправить common/template.tplx. Например, в нём вшито название предмета на титульном листе.
