---
title: Инструкции, размещенные в Интернете
permalink: index.html
layout: home
ms.openlocfilehash: c8816b7d9de9c19fbd4c6b3f373d6e4336c6ca5a
ms.sourcegitcommit: 26c283fffdd08057fdce65fa29de218fff21c7d0
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 01/27/2022
ms.locfileid: "137908667"
---
# <a name="content-directory"></a>Каталог содержимого

Гиперссылки на каждое пошаговое руководство. Инструкторы могут использовать пошаговое руководство в качестве демонстрации во время лабораторного занятия учащихся. 

## <a name="walkthroughs"></a>Пошаговые руководства

{% assign wts = site.pages | where_exp:"page", "page.url contains '/Instructions/Walkthroughs'" %}
| Модуль | Пошаговое руководство |
| --- | --- | 
{% for activity in wts %}| {{ activity.wts.module }} | [{{ activity.wts.title }}{% if activity.wts.type %} - {{ activity.wts.type }}{% endif %}]({{ site.github.url }}{{ activity.url }}) |
{% endfor %}

