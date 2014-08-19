# UMI.Console

Консольная утилита UMI.CMS версия 0.2.0 alfa

[демо](http://shelr.tv/records/502a05089660807bfb000066)

## Установка
    support@emom.ru

## Использование
    $ umi <command> [action] [flags] [options [options [...]] [<args> [<args> [...]]

### Показать информацию о текущей UMI.CMS
    $ umi info
    
### Показать базовые типы данных
    $ umi type list -nm
* **-n** показать название
* **-m** показать модуль-метод

### Показать все типы данных
    $ umi type list -AnG
* **-A** показать все типы данных
* **-n** показать название
* **-G** показать GUID
* **-g** Узнать, помечен ли тип данных как справочник
* **-l** Узнать, заблокирован ли тип данных

### Скопировать структуру типа данных
    $ umi type cp id_sourse id_target [--group=all [--field=all]

### Move or rename gruop, field for types
    $ umi type mv --group=name|id type_id new_name|new_title -n|-t
    
### Показать информацию
    $ umi type view {typeId}
    
### Редактировать тип данных
    $ umi type edit {typeId} [--guid=null [--locked=false [--delete=false]
* **--guid** или **-g** установить GUID
* **--locked** или **-l** заблокировать
* **--delete** или **-g** удвлить

### Выборки
    $ umi sel --mode=pages --type_guid=content-page -nc
    $ umi sel --mode=objects --type_guid=content-page --type_guid=users-user -cn

### TODO docs
    $ umi element
    
### TODO docs
    $ umi restriction

### TODO docs
    $ umi file
    
### TODO docs
    $ umi backup
    
### TODO docs
    $ umi redirect
    
### TODO docs
    $ umi migrate
    
### TODO docs
    $ umi perm


### Unix pipe, показать тип данных **Раздел сайта**
    $ umi type -AG | grep root-pages | awk '{print $1}' | umi type view -A

## Ресурсы
* http://umiconsole.emom.ru/
* http://hub.umi-cms.ru/project/126/
* http://umiconsole.emom.ru/issues/
