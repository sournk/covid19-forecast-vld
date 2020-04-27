# covid19-forecast-vld
Попытка спрогнозировать развитие пандемии COVID19 для Владимирской области.

# Обновление прогноза от 2020-04-27

# Прогноз от 2020-03-31
Недавно стали популярны различные варианты математических моделей развития эпидемии. Например, опубликованы [рекомендации срочного ввода жесткого карантина в штате Иллинойс от Cornell University](https://arxiv.org/abs/2003.09564) на основе адаптированной под COVID19 модели SEIR. Медуза опубликовала [исследование доцента МГУ](https://meduza.io/feature/2020/03/30/v-moskve-vveli-zhestkie-karantinnye-mery-pohozhe-eto-pravilno-matematicheskaya-model-pokazyvaet-chto-inache-mogli-by-pogibnut-bolshe-100-tysyach-chelovek) с простыми и понятными описаниями вариантов развития и последствий при разных сценариях карантина и "шашлыков" для Москвы. Washington Post простым языком [объясняет](https://www.washingtonpost.com/graphics/2020/health/corona-simulation-russian/?fbclid=IwAR31zVclS8haqRy63Kog-xBrD0923-kbi2bKIx1NNVPaM4cgJ8Vk3SPOLdA) как распространяется вирус. Факультет Biozentrum Университета Базеля запилил свой [COVID19-scenario explorer](https://neherlab.org/covid19) все на той же SEIR модели с учетом известных сейчас свойств SARS-CoV-2. 

Я сейчас живу во Владимире. Для него найти в интернете хоть какие-то модели не получилось. Поэтому я подставил такие параметры Владимирской области в базельский [COVID19-scenario explorer](https://neherlab.org/covid19):
1. Население Владимирской области - 1,358 млн. чел.
1. Возрастное распределение принято аналогичным все стране.
1. Количество зараженных на 30.03.20 - 2.
1. Количество доступных коек в области - 11500.
1. Количество доступных ИВЛ на 17.03.20 - 426.
1. Коэффициент воспроизводства R0=3,6 (в Ухане AVG(R0)=3,3  из диапазона [2,2; 6,5], а оценка кривой заражений в РФ по 30.03.20 дает R0=3,6).
1. Инкубационный период (Lauer SA et al. Ann Intern Med 2020 Mar 10) - 5 дней.
1. Бессимптомный заразный период (Y.F.W. Chan et al., Lancet, 395, 514, 2020; J.T. Wu et al., Lancet, 395, 689, 2020) - 3 дня.
1. Длительность пребывания тяжелых пациентов в стационаре (взял из модели Cornell University) - 7 дней
1. Длительность пребывания под ИВЛ (взял из модели Cornell University) - 7 дней.
1. Возрастное распределение степени тяжести заражения принято на основе наблюдений в Китае.
1. В модель заложено влияние карантина, который начинается с 30.03.20 в довольно жестком режиме и постепенно смягчается, сохраняя все-таки социальное дистанцирование до конца эпидемии.

В итоге получились такие картинки.

![Графики](/images/2020-03-31-pic001.png)
![Итоги пандемии для Владимрской области](/images/2020-03-31-pic002.png)
![Итоги пандемии для Владимрской области в распределении по возрастам](/images/2020-03-31-pic003.png)
![Параметры модели №1 - Вирус и готовность области](/images/2020-03-31-pic004.png)
![Параметры модели №2 - Самоизоляция](/images/2020-03-31-pic005.png)
![Параметры модели №3 - Влияние вируса по возратам](/images/2020-03-31-pic006.png)

Все описанное не является прогнозом, предсказанием и тем более руководством к действию. Это лишь мое видение развития ситуации исходя из моего представления текущей состояния и хоть сколько-нибудь формализованного, пусть и сильно упрощенного инструмента прогнозирования эпидемий и действия мер по их подавлению - модели SEIR. Возможно параметры модели неверные и все окажется гораздо мягче, а пока - ОСТАВАЙТЕСЬ ДОМА!

# Ссылки
1. Моделирование эпидемий. SIR модель. Simulating an epidemic
1. COVID-19 dynamics with SIR model https://www.lewuathe.com/covid-19-dynamics-with-sir-model.html
1. Модель Медузы https://meduza.io/feature/2020/03/30/v-moskve-vveli-zhestkie-karantinnye-mery-pohozhe-eto-pravilno-matematicheskaya-model-pokazyvaet-chto-inache-mogli-by-pogibnut-bolshe-100-tysyach-chelovek
1. SEIR простым языком от Washington Post https://www.washingtonpost.com/graphics/2020/health/corona-simulation-russian/?fbclid=IwAR31zVclS8haqRy63Kog-xBrD0923-kbi2bKIx1NNVPaM4cgJ8Vk3SPOLdA
1. Эпидемия в больших и малых городах https://meduza.io/feature/2020/03/30/epidemiyu-koronavirusa-zhdut-v-bolshih-gorodah-no-osnovnoy-udar-mozhet-priytis-na-stareyuschie-regiony?utm_source=telegram&utm_medium=live&utm_campaign=live
1. Модель на основе статистики перемещений людей https://habr.com/ru/company/tuturu/blog/494700/
1. COVID19 дашборд https://gisanddata.maps.arcgis.com/apps/opsdashboard/index.html#/bda7594740fd40299423467b48e9ecf6
1. Карта распространения https://yandex.ru/web-maps/covid19?ll=41.775580%2C54.894027&z=3
1. Карта самоизоляции https://yandex.ru/web-maps/covid19/isolation?ll=39.311184%2C55.398151&z=7.9 
	

#StayHome #StayAtHome #СидимДома #Самоизоляция #SocialDistansing

