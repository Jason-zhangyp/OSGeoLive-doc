:Автор: Pieter De Graef
:Версия: osgeo-live4.0
:Лицензия: Creative Commons Attribution-ShareAlike 3.0 Unported  (CC BY-SA 3.0)

.. image:: /images/project_logos/logo-geomajas.png
  :width: 50px
  :height: 50px
  :alt: Логотип проекта
  :align: right
  :target: http://www.geomajas.org

.. image:: /images/logos/OSGeo_project.png
  :scale: 100 %
  :alt: OSGeo Project
  :align: right
  :target: http://www.osgeo.org

********************************************************************************
Начало работы с Geomajas
********************************************************************************

Запуск
================================================================================

Geomajas — это фреймворк для разработки геопространственных веб-приложений. Соответственно, 
примеры на данном LiveDVD являются приложениями, построенными с использованием 
технологий Geomajas.

.. image:: /images/screenshots/1024x768/geomajas_1024x768_screen1.png
  :scale: 50%
  :alt: Демонстрация Geomajas
  :align: right

* Перейдите в каталог "Browser Clients" на рабочем столе.

* Щёлкните по ярлыку "Start Geomajas". Запустится браузер Firefox, который автоматически перейдёт по нужному адресу.

* Слева вы увидите список коротких примеров функционала, который Geomajas поддерживает "из коробки". Щёлкая по ним, вы будете открывать соответствующие примеры.

* Справа вы можете найти описания/разъяснения для каждого примера. Рекомендуется прочитать их для лучшего понимания.


Создание новых Geomajas-приложений
================================================================================

Для создания нового Geomajas-приложения вам потребуется `Maven <http://maven.apache.org/>`_ ::

    $ sudo apt-get install maven2

Maven — это инструмент для сборки и управления проектами на базе Java. 
У Geomajas описан архетип для Maven, устанавливающий исходное приложение одной командой::

    $ mvn archetype:generate -DarchetypeCatalog=http://files.geomajas.org/archetype-catalog.xml

Поздравляем, вы только что создали новое Geomajas-приложение!
Вы можете запустить его сейчас или открыть среду разработки. 
Для запуска приложения перейдите в каталог приложения (где находится 
pom.xml) и выполните следующую команду Maven::

    $ mvn jetty:run

Приложение будет скомпилировано и запущено в контейнере *jetty*. 
Доступ к приложению вы можете получить по следующему url:
http://localhost:8080/

Для дополнительной информации о создании Geomajas-приложений или об установке среды разработки 
смотрите `Geomajas getting started <http://files.geomajas.org/maven/trunk/geomajas/docbook-gettingstarted/html/master.html#prereq>`_.

Для основной информации смотрите `Домашнюю страницу Geomajas <http://www.geomajas.org/>`_.

