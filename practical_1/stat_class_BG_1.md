Упражнение 1
================
ас.д-р К. Костадинов
21.09.2021 г

# Вместо увод

## Защо учим статистика?

-   Статистиката е метод който използваме за да превърнем данните в
    информация.
-   Информацията, която получима се превръща в знание.
-   Знанието се въвежда в ежедневната медицинска практика, чрез клинични
    наръчници или политики в общественото здравеопазване.
-   По пътя на тази логическа верига, дори и малко нескромно,
    статистиката е метод, който пряко помага, както на пациента, като и
    на здравето на обществото.

## С какво ще ни помогне статистиката?

-   Да взимаме информирани решения в ежедневната ни практика.
-   Да взимаме най-добрите решения базирани на доказателства за политики
    в общественото здравеопазване.
-   Да разберем как работи науката.
-   За да четем критично нова научна информация.
-   За да сме по добри лекари.

## Какво няма да научим?

Понастоящем статистиката е силен инструмент в т.н “наука за данните”
(data science). В съчетание със сложна математика, програмиране и доза
креативност тази нова дисциплина решава редица практически задачи чрез
използване на компютърни технологии. В момента дори има разработени
скенери които “сами разчитат” дали има заболяване и с изчислена възможна
“грешка” класифицират какво е то. Това е възможно именно заради
инструментите, които статистиката ни предоставя. Разработени са и
електрокардиографи записващи сърдечната дейност на пациента и
“автоматично” разпознаващи дали е налице определено заболяване. В този
курс, обаче целта е да придобиете най-основите знания за това как работи
статистиката, каква е логиката в нея и какъв език използва.

# Упражнение 1

Преди да започнем със задачата за това упражнение, следва да се
запознаем с някои основни понятия в статистиката:

## Терминология

В статистиката един от най-сложните елементи за студента са `термините`.
За да “не сме изгубени в превода” в упражненията, ще въвеждаме тези
термини с някои основни примери. Опитайте се след всяко упражнения и
лекция да преговорите тези термини. Съшо така се опитайте да си дадете
собствен пример за някой от тях, ако не успявате, следва да изясните
този термин възможно най-скоро. Много вероятно е някой от тези думички
да бъде използвана отново за да се обяснят по-сложни концепции в
следващите ни занятия. `Вероятно` произхожда от `вероятност` и това е
много важен термин който ще изясним в следващите ни упражнения.

-   `абсолютни величини`

Това са абсолютни **числа**, които количествено характеризират обемите
на статистическите съвкупности или на части от тях, както и значенията
на статистическите признаци.

Те са винаги **наименовани числа**, измерени в съответните **мерни
единици** . Статистическите изследвания обикновено започват с анализ на
абсолютни величини, но този тип величини **не са достатъчни** за
директни сравнения в **пространствено-времеви аспект.**

За да звучи достъпно, нека използваме *пример*. Систолното артериално
налягане измерено в mmHg е абсолютна величина- има абсолютна стойност,
мерна единица и количествено характеризира систолното артериалното
налягане. Кръвната захар измерена в mmol/l също е абсолютна величина -
отново е число отразяващо количествено определен признак.

-   `относителни величини`

Те се изчисляват се като частно от делението на две абсолютни величини.
Представят като коефициенти, в проценти (когато коефициентът се умножи
по 100), в промили (когато коефициентът се умножи по 1000) и т.н.

В медицината често използваме относителни величини, *например* когато
измерваме помената функция на сърцето можем да използваме за показател
колко милилитра кръв постъпват в аортата след една систола (ударен
обем). Това е абсолютна величина - има мерна единица (ml) и
характеризира сърдечната дейност. Логично е хората с по-висок ръст и
тегло (по-едро телосложение) ще имат по-високи стойности за този
показател отколкото хората с по-нисък ръст и по-малко тегло. Също е
логично сърцето на състезател по сумо да изпомпва по-голямо количество
кръв (в милилитри) спрямо сърцето на първокласник. Означава ли това, че
сърцето на състезателя по сумо работи по-добре от това на първокласника?
Отговорът е, че не можем да преценим - двете абсолютни величини не са
достатъчни за сравнение. Затова по-важното в случая е какво е
съотношението на ударният обем, спрямо количеството кръв налично в
сърцето в края на диастолата. Това е т.н “фракция на изтласкване” и
представлява `относителна величина`. Понеже е отношение на две числа,
когато умножим това отношение х 100 получаваме “%”.

-   `екстензивни показатели`

Наричат се още **структурни** и показват как явлението се разпределя на
съставните му части, когато то се разглежда самостоятелно само за себе
си в определено време и място. *Например* ако приемем “възрастта” в гр.
Пловдив за “явление” можем да представим всички жители на град Пловдив в
категории според възрастовата им група: новородени до 1г., между 1 и 5
год., от 5 до 10г. и т.н. Ако изчислим броя на хората в съответната
възрастовата група спрямо всички жители на града ще получим
`екстензивен показател` .

![](stat_class_BG_1_files/figure-gfm/figure%201-1.png)<!-- -->

Както се вижда от фигурата, най-голяма е пропорцията на жителите във
възрастта от 40 до 44 год. Тази пропорция е част от всички жители на
град на Пловдив. Това същността на екстензивния показател- едно явление,
в случая възрастта в конкретно място (гр. Пловдив) в конкретна година
(2020) разложено на съставните му части (възрастовите периоди пред 5
годишен интервал)

-   `интензивни показатели`

Te се наричат се още **честотни** и показват колко често се среща дадено
явление в свойствената му среда. Всяка относителна величина е отношение
между обемите на две различни статистически съвкупности, но намиращи се
във връзка помежду си. В числителя е явлението, а в знаменателя е
абсолютният обем на средата, в която възниква определеното събитие.

За да разберем какво е интензивен показател ще дадем един негов
представител, често използван в медицината (още по-често неизползван,
когато трябва да бъде използван). Това е показателя *леталитет*.

`Леталитет` е показател представяш броя смъртни случаи от конкретно
заболяване върху броя на болните от това заболяване в за конкретен
период от време и място. *Например* леталитет при заболяването морбили
(дребна шарка) при деца (до 18г.) е 5%. Това означава, че теоретично, на
100 деца със заболяването (дребна шарка) 5 са с летален изход. Тези 5%
всъщност показват **честотата** на смъртни случаи при деца болни с
дребна шарка- тоест честотата на явлението в неговата свойствена среда.
В числителя на този показател постояваме броя смъртни случаи- това е
явлението, докато в знаменателя поставяме броя болни деца с морбили-
това е обема на средата в която се проявява явлението. На практика
числителят и знаменателя представляват две различни статистически
съвкупности, въпреки това те има връзка помежду си.

`Смъртността` е показател представяш броя на починалите спрямо средния
брой население в конкретната област и за конкретно време и не бива да се
бърка с `леталитет`.

В социалната медицина, епидемиологията и статистиката се ползват
множество такива показатели. **Например** `заболеваемост` , представлява
съотношението на броя новозаболели от някакво заболяване (например от
рак на гърдата) спрямо популацията в риск (всички, които биха могли да
се разболеят от това заболяване) за даден период от време. В 3-ти курс
ще се запознаете с още много подобни показатели, но е важно да знаете
тяхната идея. Използваме тези показатели за да оцененим определени
здравни явления, да ги измерим количествено (с някаква цифра), да можем
да ги сравняваме както в различни периоди, така и между различни държави
например.

В ежедневната практика като лекари също ще ползвате подобни `интензивни`
показатели. *Например* при пациенти с белодробна астма, вида на
използваното лечение зависи от честотата на екзацербации (обостряния)
т.н “exacerbation rate”. Това отново е `интензивен` показател.

## Пряк метод на стандартизация

Преди да прочетете определението за стандартизация, нека започнем с един
пример. Понеже това упражнение няма претенцията за академичен учебник,
нека си представим, че от днес ние сме състава на Министерство на
здравеопазването. Вие - министър , а аз ваш съветник със скромна
държавна залата. Изправени сме пред сериозен проблем: В държавата
върлува много опасен вирус (много по-опасен от COVID-19). Имаме ваксина,
но липса на доверие в нея. Много хора вярват, че ваксините дори убиват.
Днес след среща с граждани, противопоставящи се на ваксините, получавате
научна статия. Чрез нея, противниците на ваксините се опитват да ви
убедят, че ваксините са вредни. В нашият пример приемаме, че този нов
вирус може да засегне всички ни еднакво.

В `таблицата 1` можете да видите данните от тази научна публикация.

<div id="tebfvwcxlo" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">

 
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="3" class="gt_heading gt_title gt_font_normal" style>Табл.1. Опасни ваксини</th>
    </tr>
    <tr>
      <th colspan="3" class="gt_heading gt_subtitle gt_font_normal gt_bottom_border" style>неизветсен източник</th>
    </tr>
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_left" rowspan="1" colspan="1">type</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td class="gt_row gt_left">vaccinated</td>
<td class="gt_row gt_right">4000</td>
<td class="gt_row gt_right">2850</td></tr>
    <tr><td class="gt_row gt_left">unvaccinated</td>
<td class="gt_row gt_right">8000</td>
<td class="gt_row gt_right">5500</td></tr>
  </tbody>
  
  
</table>
</div>

Таблицата е базирана на научно изследване във Великобритания. Авторът
посочва, че от 4000 ваксинирани са починали 2850 души, докато при
неваксинираните 8000 души са починали 5500. Тези числа всъщност
представляват `абсолютни величини`. За да се опитаме да ги сравним, ще
трябва да използваме `относителни величини`. Тоест каква пропорция от
ваксинираните са починали, същата пропорция от неваксинираните."
Сметката " тук е лесна : трябва да разделим броя на починалите
ваксинирани върху общият брой ваксинирани, както и броя на починалите
неваксинирани, спрямо общият брой неваксинирани. В резултат ще получим
`относителна величина` която също така ще представлява и
`интензивен показател`.

![](stat_class_BG_1_files/figure-gfm/unnamed-chunk-6-1.png)<!-- -->

Тук резултатът е изненада. Оказва се, че в групата на ваксинираните
71.2% са починали, докато при неваксинираните починали са 68.8%. Това е
разлика от 2,4 процентни пункта (важно простите аритметични операции
между проценти се изразяват в процентни пунктове). Може би наистина
“антиваксарите” имат право. Статията изглежда достоверна. Имаме толкова
много наблюдавани хора и изглежда, че сред ваксинираните имаме повече
починали.

Как бихме могли да си обясним този резултат? Нима наистина ваксините са
причина за по-големия брой смъртни случай? Трябва ли да продължим да
използваме тази ваксина, ако решението зависеше от нас? Бихме ли
посъветвали пациентите си да се ваксинират?

Преди да дадем категоричното си решение, можем малко да помислим върху
данните. Те все още не са информация на която да базираме решенията си.
В случая можем да разглеждаме цифрите в таблицата, като сурови данни
измерващи една връзка. Тази връзка е между ваксинацията и леталният
изход. Не изглежда логично смъртта да се причинява единствено от
ваксината или липсата на такава. Има редица други фактори, които влияят
на смъртта - придружаващи заболявания, предоставената медицинска помощ и
може би най-важният сред тях- ВЪЗРАСТТА. Нормално е, ако хората включени
в изследването са по-възрастни то да наблюдаваме и по-вече починали.

За да проверим дали възрастта “замъглява” връзката между ваксинацията и
смъртта можем да използваме статистическия метод на стандартизацията.

При сравняването на интензивни статистически показатели се наблюдава
фактът, че величината на тези показатели стои в зависимост от
структурата на средата, в която изучаваните явления се проявяват.
Например раждаемостта е по-висока в онези населени места, в които
преобладава население на възраст 20-30 г. При този и други случаи,
когато трябва да се сравняват интензивни статистически показатели,
изчислени от среда с различна структура, е необходимо да бъде приложен
т.нар. метод на стандартизация.

### Определение

-   Под `стандартизация` се разбира способът за преобразуване на общите
    коефициенти, позволяващ да се отстрани или елиминира влиянието на
    възрастовите или други различия в състава на сравняваните групи.
    `Стандартизираните` показатели позволяват да се анализира и оцени
    нивото на изучаваното явление при създадени `условия на еднородност`
    в сравняваните групи и показват какви биха били общите коефициенти в
    сравняваните групи, ако тези групи имаха `еднакъв състав.`

Отново поглеждайки нашият пример - възможно е да се окаже, че в групата
на ваксинираните са предпочетени повече възрастни хора, докато при
неваксинираните са повече младите. Това би обяснило тези резултати.
`Стандартизацията` е метод, които ще създаде възможност да сравним тези
две групи, след като премахнем действието на възрастта като “замъгляващ
фактор” в тази данни.

### Стъпки

За да извършим стандартизация (в курса по статистика се спираме
единствено и само на прекия метод за стандартизация) следва да
разполагаме с повече данни. Таблицата която разгледахме не съдържа
информация за възрастта на участниците. Затова след запитване към
авторът на публикацията получаваме по-подробни данни - които можете да
видите в таблица 2.

<div id="ufsykesusv" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#ufsykesusv .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#ufsykesusv .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#ufsykesusv .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#ufsykesusv .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#ufsykesusv .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ufsykesusv .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#ufsykesusv .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#ufsykesusv .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#ufsykesusv .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#ufsykesusv .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#ufsykesusv .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#ufsykesusv .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#ufsykesusv .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#ufsykesusv .gt_from_md > :first-child {
  margin-top: 0;
}

#ufsykesusv .gt_from_md > :last-child {
  margin-bottom: 0;
}

#ufsykesusv .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#ufsykesusv .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#ufsykesusv .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#ufsykesusv .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#ufsykesusv .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#ufsykesusv .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#ufsykesusv .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#ufsykesusv .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ufsykesusv .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#ufsykesusv .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#ufsykesusv .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#ufsykesusv .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#ufsykesusv .gt_left {
  text-align: left;
}

#ufsykesusv .gt_center {
  text-align: center;
}

#ufsykesusv .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#ufsykesusv .gt_font_normal {
  font-weight: normal;
}

#ufsykesusv .gt_font_bold {
  font-weight: bold;
}

#ufsykesusv .gt_font_italic {
  font-style: italic;
}

#ufsykesusv .gt_super {
  font-size: 65%;
}

#ufsykesusv .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="3" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Табл.2. Ваксинирани и неваксинирани повъзрастови групи</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">age_group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_number</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr class="gt_group_heading_row">
      <td colspan="3" class="gt_group_heading">unvaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">4000</td>
<td class="gt_row gt_right">2400</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1400</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">800</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">900</td></tr>
    <tr class="gt_group_heading_row">
      <td colspan="3" class="gt_group_heading">vaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">250</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">300</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">700</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1600</td></tr>
  </tbody>
  
  
</table>
</div>

Сега вече имаме повече данни не само за това колко са били ваксинирани и
колко не са, но и в каква възрастова група попадат. Може би, ви прави
впечатление, че ваксинираните са предимно по-възрастни хора, докато при
неваксинираните по-младите. Както можете да забележите от фигурата - във
групата до 24г. преобладат неваксинирани, докато при над 45-годинишните
ваксинираните. Можем да преминем към стъпка 1

![](stat_class_BG_1_files/figure-gfm/unnamed-chunk-10-1.png)<!-- -->

#### Стъпка 1 Изчисляваме нестандартизираните интензивни показатели

Както по-рано, така и сега, можем да изчислим какъв процент от
участниците в двете групи са починали. Това става като разделим броя на
починалите върху броя на участниците. В случая ще изчислим този
показател за всяка една възрастова група. След тези калкулации
получаваме:

<div id="lcrcexfdxn" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#lcrcexfdxn .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#lcrcexfdxn .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#lcrcexfdxn .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#lcrcexfdxn .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#lcrcexfdxn .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#lcrcexfdxn .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#lcrcexfdxn .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#lcrcexfdxn .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#lcrcexfdxn .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#lcrcexfdxn .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#lcrcexfdxn .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#lcrcexfdxn .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#lcrcexfdxn .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#lcrcexfdxn .gt_from_md > :first-child {
  margin-top: 0;
}

#lcrcexfdxn .gt_from_md > :last-child {
  margin-bottom: 0;
}

#lcrcexfdxn .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#lcrcexfdxn .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#lcrcexfdxn .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#lcrcexfdxn .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#lcrcexfdxn .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#lcrcexfdxn .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#lcrcexfdxn .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#lcrcexfdxn .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#lcrcexfdxn .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#lcrcexfdxn .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#lcrcexfdxn .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#lcrcexfdxn .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#lcrcexfdxn .gt_left {
  text-align: left;
}

#lcrcexfdxn .gt_center {
  text-align: center;
}

#lcrcexfdxn .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#lcrcexfdxn .gt_font_normal {
  font-weight: normal;
}

#lcrcexfdxn .gt_font_bold {
  font-weight: bold;
}

#lcrcexfdxn .gt_font_italic {
  font-style: italic;
}

#lcrcexfdxn .gt_super {
  font-size: 65%;
}

#lcrcexfdxn .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="4" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Табл.3. Ваксинирани и неваксинирани повъзрастови групи</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">age_group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_number</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_unstandardized</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr class="gt_group_heading_row">
      <td colspan="4" class="gt_group_heading">unvaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">4000</td>
<td class="gt_row gt_right">2400</td>
<td class="gt_row gt_right">60</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1400</td>
<td class="gt_row gt_right">70</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">800</td>
<td class="gt_row gt_right">80</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">900</td>
<td class="gt_row gt_right">90</td></tr>
    <tr class="gt_group_heading_row">
      <td colspan="4" class="gt_group_heading">vaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">250</td>
<td class="gt_row gt_right">50</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">300</td>
<td class="gt_row gt_right">60</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">700</td>
<td class="gt_row gt_right">70</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1600</td>
<td class="gt_row gt_right">80</td></tr>
  </tbody>
  
  
</table>
</div>

В `таблица 3` колона `fatality_rate_unstandardized` представлява
нестандартизираният показател във всяка една от възрастовите групи за
ваксинираните и неваксинираните. Тук е важно да запомним, че общият
нестандартизиран показател не е сума от резултатите по подгрупи. Не
можем да сумираме тези показатели за ваксинирани и неваксинирани и да ги
сравним.

#### Стъпка 2 Изчисляване на “стандарта”

За да можем да сравним двете групи, трябва да “стандартизираме”
получените по групови показатели. Само след стандартизация е възможно да
сумиране получените числа по възрастови групи и да сравним ваксинирани
срещу неваксинирани. За да направим това е необходимо да изберем
възрастовата структура една от тези две групи за **стандарт**.

Тук, често възниква въпроса коя структура да изберем за стандарт? Защо
да предпочетем едната спрямо другата? Какво е правилото? Всъщност
отговорът на всички тези въпроси е че няма особено значение. Разбира се,
че числата след стандартизация ще са различни в зависимост коя структура
сме избрали за стандарт, но тук стойността на тези числа не е от толкова
голямо значение. От значение е коя от сумарните стойности е по-висока.
Независимо коя група сме избрали за стандарт, тази разлика остава една и
съща. Това е - независимо коя група изберем за “стандартна” то извода
няма да се промени. В това упражнение ще докажем това, като извършим
стандартизацията, като вземем за стандарт първо структурата на
неваксинираните, а после решим същият пример, като вземем за стандарт
структурата на ваксинираните.

Следващият въпрос, които вероятно възниква е “какво означава да вземем
за стандарт структурата на неваксинираните?”. Отговорът е логичен: ако
разгледаме само включените участници, които не са ваксинирани можем да
изчислим тяхната възрастова структура- ще използваме броя на участниците
в определена възрастова група за числител, а общия брой неваксинирани за
знаменател. Така сред като изчислим какъв процент участници имаме във
всяка възрастова група ще получим `екстензивен коефициент` който ще
ползваме за да стандартизираме `интензивните показатели` за всяка една
от възрастовите групи.

Това сме направили в `таблица 4`. Първо сме изчислили “стандарта” за
участниците под 24г. - те са 4000, спрямо общият брой неваксинирани
8000. Получаваме 0.5 (ако умножим по 100 ще получим %, т.е. участниците
до 24 години) са половината от всички участници. Това ще използваме за
стандарт както за ваксинираните така и за неваксинираните. По подобен
начин сме получили и стандарта за възрастовата група от 25 до 34г. В
групата на неваксинираните те са 2000, което представлява 25% (или 0.25)
от всички неваксинирани. Тази стойност 0.25 ще използваме за стандарт за
всички участници от 25 до 34г. - ваксинирани и неваксинирани. Това е
логиката при всеки един от тези коефициенти в таблица 4. Може да ви
направи впечатление, че сбора на всички стандарти е равен на 1-ца (тоест
100%). Това е така защото този стандарт всъщност е `екстензивен`
показател - показва как се разлага явлението “възраст” на съставните и
части- отделните възрастови групи.

<div id="gtzsoxxewb" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#gtzsoxxewb .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#gtzsoxxewb .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#gtzsoxxewb .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#gtzsoxxewb .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#gtzsoxxewb .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#gtzsoxxewb .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#gtzsoxxewb .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#gtzsoxxewb .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#gtzsoxxewb .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#gtzsoxxewb .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#gtzsoxxewb .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#gtzsoxxewb .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#gtzsoxxewb .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#gtzsoxxewb .gt_from_md > :first-child {
  margin-top: 0;
}

#gtzsoxxewb .gt_from_md > :last-child {
  margin-bottom: 0;
}

#gtzsoxxewb .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#gtzsoxxewb .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#gtzsoxxewb .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#gtzsoxxewb .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#gtzsoxxewb .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#gtzsoxxewb .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#gtzsoxxewb .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#gtzsoxxewb .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#gtzsoxxewb .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#gtzsoxxewb .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#gtzsoxxewb .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#gtzsoxxewb .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#gtzsoxxewb .gt_left {
  text-align: left;
}

#gtzsoxxewb .gt_center {
  text-align: center;
}

#gtzsoxxewb .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#gtzsoxxewb .gt_font_normal {
  font-weight: normal;
}

#gtzsoxxewb .gt_font_bold {
  font-weight: bold;
}

#gtzsoxxewb .gt_font_italic {
  font-style: italic;
}

#gtzsoxxewb .gt_super {
  font-size: 65%;
}

#gtzsoxxewb .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="5" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Таблица 4. Изчисляване на стандарта спрямо групата на неваксинираните</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">age_group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_number</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_unstandardized</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">standard_unvaccinated</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">4000</td>
<td class="gt_row gt_right">2400</td>
<td class="gt_row gt_right">60</td>
<td class="gt_row gt_right">0.500</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1400</td>
<td class="gt_row gt_right">70</td>
<td class="gt_row gt_right">0.250</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">800</td>
<td class="gt_row gt_right">80</td>
<td class="gt_row gt_right">0.125</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">900</td>
<td class="gt_row gt_right">90</td>
<td class="gt_row gt_right">0.125</td></tr>
  </tbody>
  
  
</table>
</div>

#### Стъпка 3: Изчисляване на стандартизираните показатели за заболеваемост

След като имаме “стандарт”, можем да пристъпим към следващата стъпка.
Смъртността която изчислихме в таблица 3, беше нестандартизирана. Сега е
момента да използваме “стандарта” от стъпка 2 и да я стандартизираме.
Как става това? Решението е лесно: за всяка една от възрастовите групи
умножаваме нестандартизирания показател по стандарта.

<div id="vsilucxoms" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#vsilucxoms .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#vsilucxoms .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#vsilucxoms .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#vsilucxoms .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#vsilucxoms .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#vsilucxoms .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#vsilucxoms .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#vsilucxoms .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#vsilucxoms .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#vsilucxoms .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#vsilucxoms .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#vsilucxoms .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#vsilucxoms .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#vsilucxoms .gt_from_md > :first-child {
  margin-top: 0;
}

#vsilucxoms .gt_from_md > :last-child {
  margin-bottom: 0;
}

#vsilucxoms .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#vsilucxoms .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#vsilucxoms .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#vsilucxoms .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#vsilucxoms .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#vsilucxoms .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#vsilucxoms .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#vsilucxoms .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#vsilucxoms .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#vsilucxoms .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#vsilucxoms .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#vsilucxoms .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#vsilucxoms .gt_left {
  text-align: left;
}

#vsilucxoms .gt_center {
  text-align: center;
}

#vsilucxoms .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#vsilucxoms .gt_font_normal {
  font-weight: normal;
}

#vsilucxoms .gt_font_bold {
  font-weight: bold;
}

#vsilucxoms .gt_font_italic {
  font-style: italic;
}

#vsilucxoms .gt_super {
  font-size: 65%;
}

#vsilucxoms .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="6" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Таблица 5. Изчисляване на стандартизираните показатели</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">age_group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_number</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_unstandardized</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">standard_unvaccinated</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_standardized</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr class="gt_group_heading_row">
      <td colspan="6" class="gt_group_heading">unvaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">4000</td>
<td class="gt_row gt_right">2400</td>
<td class="gt_row gt_right">60</td>
<td class="gt_row gt_right">0.500</td>
<td class="gt_row gt_right">30.00</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1400</td>
<td class="gt_row gt_right">70</td>
<td class="gt_row gt_right">0.250</td>
<td class="gt_row gt_right">17.50</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">800</td>
<td class="gt_row gt_right">80</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">10.00</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">900</td>
<td class="gt_row gt_right">90</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">11.25</td></tr>
    <tr class="gt_group_heading_row">
      <td colspan="6" class="gt_group_heading">vaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">250</td>
<td class="gt_row gt_right">50</td>
<td class="gt_row gt_right">0.500</td>
<td class="gt_row gt_right">25.00</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">300</td>
<td class="gt_row gt_right">60</td>
<td class="gt_row gt_right">0.250</td>
<td class="gt_row gt_right">15.00</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">700</td>
<td class="gt_row gt_right">70</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">8.75</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1600</td>
<td class="gt_row gt_right">80</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">10.00</td></tr>
  </tbody>
  
  
</table>
</div>

Сега сме почти готови- имаме стандартизираните показатели като сме
умножили интензивните показатели за смъртност
`fatality_rate_unstandardized` по квотата за стандарт
`standard_unvaccinated`. Тази квота всъщност беше възрастовата структура
на групата неваксинирани (нея избрахме за стандарт). Вече знаете, че
нестандартизираните показатели не се събират (това го питат на изпит
чувам). За сметка на това стандартизираните могат да бъдат събирани-
защото иначе цялата тази математическа главоблъсканица би била излишна.
Когато съберем стандартизираните показатели по възрастови групи ще
получим стандартизирания интензивен показател за смъртността - както за
ваксинирани така и за неваксинирани. Този показател е стандартизиран за
възрастта. Тоест, сме избегнали “замъгляващият ефект” на това, че са
ваксинирани предимно възрастни хора, а неваксинирани са преидмно млади.

Нека извършим тази последна калкулация. За групата на ваксинираните това
означава да съберем `25%` (смъртността в тази група при ваксинирани) +
`15%` (във възрастовата група 25-34г.) + `8.75 %`(35-44г.) + `10%` (за
тези над 45г.). Получаваме `58.75%`. Тук следва да направим същото и за
групата на неваксинираните. За тях сборът е `65.75%.` фиг. 6 ги показва
по-систематично.

<div id="qftyscekze" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#qftyscekze .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#qftyscekze .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#qftyscekze .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#qftyscekze .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#qftyscekze .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#qftyscekze .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#qftyscekze .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#qftyscekze .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#qftyscekze .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#qftyscekze .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#qftyscekze .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#qftyscekze .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#qftyscekze .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#qftyscekze .gt_from_md > :first-child {
  margin-top: 0;
}

#qftyscekze .gt_from_md > :last-child {
  margin-bottom: 0;
}

#qftyscekze .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#qftyscekze .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#qftyscekze .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#qftyscekze .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#qftyscekze .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#qftyscekze .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#qftyscekze .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#qftyscekze .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#qftyscekze .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#qftyscekze .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#qftyscekze .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#qftyscekze .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#qftyscekze .gt_left {
  text-align: left;
}

#qftyscekze .gt_center {
  text-align: center;
}

#qftyscekze .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#qftyscekze .gt_font_normal {
  font-weight: normal;
}

#qftyscekze .gt_font_bold {
  font-weight: bold;
}

#qftyscekze .gt_font_italic {
  font-style: italic;
}

#qftyscekze .gt_super {
  font-size: 65%;
}

#qftyscekze .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="2" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Таблица 6. Сравнение на стандартизираните показатели</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_fatality_rate_standardized</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td class="gt_row gt_center">unvaccinated</td>
<td class="gt_row gt_right">68.75</td></tr>
    <tr><td class="gt_row gt_center">vaccinated</td>
<td class="gt_row gt_right">58.75</td></tr>
  </tbody>
  
  
</table>
</div>

#### Стъпка 4: Заключение

Стандартизираните показатели за заболеваемост в двете групи са съответно
`58.75%` и `68.75%`. Заболеваемостта сред неваксинираните, е с 10%
по-висока. (Обърнете внимание тук разликата между проценти остава също
процент, а не процентен пункт. Причината за това е защото тези
показатели са стандартизирани- тоест сме “изравнили” тяхната структура,
в случая възрастова структура.)

![](stat_class_BG_1_files/figure-gfm/unnamed-chunk-20-1.png)<!-- -->

Предполагам, обаче някои от вас се питат, какво би се случило, ако не
ползваме за стандарт възрастовата структура на неваскинираните. Защо
избрахме точно нея? Това не е ли пристрастие?

За да докажем, че за изводът няма значение коя структура използваме, ще
решим отново примера, като този път за стандарт, използваме структурата
на ваксинираните. Отново от стъпка 2.

#### Стъпка 2 Изчисляваме стандарта (този път спрямо ваксинираните)

В този случай за да изчислим стандарта започваме, като гледаме таблицата
само за ваксинираните. В нея установяваме, че участниците под 24г. са
500 от общо 4000. Това означава, че стандарта е 0.125 (или 12.5%). Това
извършваме за всяка една от възрастовите групи. Резултатът е видим в
таблица 7.

<div id="kapqmozcpl" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#kapqmozcpl .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#kapqmozcpl .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#kapqmozcpl .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#kapqmozcpl .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#kapqmozcpl .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kapqmozcpl .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#kapqmozcpl .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#kapqmozcpl .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#kapqmozcpl .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#kapqmozcpl .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#kapqmozcpl .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#kapqmozcpl .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#kapqmozcpl .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#kapqmozcpl .gt_from_md > :first-child {
  margin-top: 0;
}

#kapqmozcpl .gt_from_md > :last-child {
  margin-bottom: 0;
}

#kapqmozcpl .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#kapqmozcpl .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#kapqmozcpl .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#kapqmozcpl .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#kapqmozcpl .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#kapqmozcpl .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#kapqmozcpl .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#kapqmozcpl .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#kapqmozcpl .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#kapqmozcpl .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#kapqmozcpl .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#kapqmozcpl .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#kapqmozcpl .gt_left {
  text-align: left;
}

#kapqmozcpl .gt_center {
  text-align: center;
}

#kapqmozcpl .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#kapqmozcpl .gt_font_normal {
  font-weight: normal;
}

#kapqmozcpl .gt_font_bold {
  font-weight: bold;
}

#kapqmozcpl .gt_font_italic {
  font-style: italic;
}

#kapqmozcpl .gt_super {
  font-size: 65%;
}

#kapqmozcpl .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="5" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Таблица 7. Изчисляване на стандарта спрямо групата на ваксинираните</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">age_group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_number</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_standardized</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">standard_unvaccinated</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">250</td>
<td class="gt_row gt_right">50</td>
<td class="gt_row gt_right">0.125</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">300</td>
<td class="gt_row gt_right">60</td>
<td class="gt_row gt_right">0.125</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">700</td>
<td class="gt_row gt_right">70</td>
<td class="gt_row gt_right">0.250</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1600</td>
<td class="gt_row gt_right">80</td>
<td class="gt_row gt_right">0.500</td></tr>
  </tbody>
  
  
</table>
</div>

#### Повтаряме Стъпка 3: Изчисляване на стандартизираните показатели за заболеваемост

След като имаме “стандарт”, този път спрямо групата на ваксинираните
можем да пристъпим отново към стъпка 3. Сега е момента да използваме
“стандарта” от новата стъпка 2. Решението отново е лесно: за всяка една
от възрастовите групи умножаваме нестандартизирания показател по
стандарта.

<div id="ewxghuxcdv" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#ewxghuxcdv .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#ewxghuxcdv .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#ewxghuxcdv .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#ewxghuxcdv .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#ewxghuxcdv .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ewxghuxcdv .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#ewxghuxcdv .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#ewxghuxcdv .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#ewxghuxcdv .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#ewxghuxcdv .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#ewxghuxcdv .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#ewxghuxcdv .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#ewxghuxcdv .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#ewxghuxcdv .gt_from_md > :first-child {
  margin-top: 0;
}

#ewxghuxcdv .gt_from_md > :last-child {
  margin-bottom: 0;
}

#ewxghuxcdv .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#ewxghuxcdv .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#ewxghuxcdv .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#ewxghuxcdv .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#ewxghuxcdv .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#ewxghuxcdv .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#ewxghuxcdv .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#ewxghuxcdv .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#ewxghuxcdv .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#ewxghuxcdv .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#ewxghuxcdv .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#ewxghuxcdv .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#ewxghuxcdv .gt_left {
  text-align: left;
}

#ewxghuxcdv .gt_center {
  text-align: center;
}

#ewxghuxcdv .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#ewxghuxcdv .gt_font_normal {
  font-weight: normal;
}

#ewxghuxcdv .gt_font_bold {
  font-weight: bold;
}

#ewxghuxcdv .gt_font_italic {
  font-style: italic;
}

#ewxghuxcdv .gt_super {
  font-size: 65%;
}

#ewxghuxcdv .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="6" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Таблица 8. Изчисляване на стандартизираните показатели</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">age_group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_number</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">deaths</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_unstandardized</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">standard_vaccinated</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">fatality_rate_standardized</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr class="gt_group_heading_row">
      <td colspan="6" class="gt_group_heading">unvaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">4000</td>
<td class="gt_row gt_right">2400</td>
<td class="gt_row gt_right">60</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">7.50</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1400</td>
<td class="gt_row gt_right">70</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">8.75</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">800</td>
<td class="gt_row gt_right">80</td>
<td class="gt_row gt_right">0.250</td>
<td class="gt_row gt_right">20.00</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">900</td>
<td class="gt_row gt_right">90</td>
<td class="gt_row gt_right">0.500</td>
<td class="gt_row gt_right">45.00</td></tr>
    <tr class="gt_group_heading_row">
      <td colspan="6" class="gt_group_heading">vaccinated</td>
    </tr>
    <tr><td class="gt_row gt_center">under 24</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">250</td>
<td class="gt_row gt_right">50</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">6.25</td></tr>
    <tr><td class="gt_row gt_center">25 to 34</td>
<td class="gt_row gt_right">500</td>
<td class="gt_row gt_right">300</td>
<td class="gt_row gt_right">60</td>
<td class="gt_row gt_right">0.125</td>
<td class="gt_row gt_right">7.50</td></tr>
    <tr><td class="gt_row gt_center">35 to 44 </td>
<td class="gt_row gt_right">1000</td>
<td class="gt_row gt_right">700</td>
<td class="gt_row gt_right">70</td>
<td class="gt_row gt_right">0.250</td>
<td class="gt_row gt_right">17.50</td></tr>
    <tr><td class="gt_row gt_center">over 45</td>
<td class="gt_row gt_right">2000</td>
<td class="gt_row gt_right">1600</td>
<td class="gt_row gt_right">80</td>
<td class="gt_row gt_right">0.500</td>
<td class="gt_row gt_right">40.00</td></tr>
  </tbody>
  
  
</table>
</div>

Логично, след като сме използвали и друг стандарт, изчислените
стандартизирани показатели са различни. Отново напомням, не се
интересуваме от конкретното число, а от заключението което ще направим.
Отново можем да сумираме стандартизираните показатели.

<div id="zmzwaouylb" style="overflow-x:auto;overflow-y:auto;width:auto;height:auto;">
<style>html {
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Helvetica Neue', 'Fira Sans', 'Droid Sans', Arial, sans-serif;
}

#zmzwaouylb .gt_table {
  display: table;
  border-collapse: collapse;
  margin-left: auto;
  margin-right: auto;
  color: #333333;
  font-size: 16px;
  font-weight: normal;
  font-style: normal;
  background-color: #FFFFFF;
  width: auto;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #A8A8A8;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #A8A8A8;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
}

#zmzwaouylb .gt_heading {
  background-color: #FFFFFF;
  text-align: center;
  border-bottom-color: #FFFFFF;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#zmzwaouylb .gt_title {
  color: #333333;
  font-size: 125%;
  font-weight: initial;
  padding-top: 4px;
  padding-bottom: 4px;
  border-bottom-color: #FFFFFF;
  border-bottom-width: 0;
}

#zmzwaouylb .gt_subtitle {
  color: #333333;
  font-size: 85%;
  font-weight: initial;
  padding-top: 0;
  padding-bottom: 6px;
  border-top-color: #FFFFFF;
  border-top-width: 0;
}

#zmzwaouylb .gt_bottom_border {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zmzwaouylb .gt_col_headings {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
}

#zmzwaouylb .gt_col_heading {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 6px;
  padding-left: 5px;
  padding-right: 5px;
  overflow-x: hidden;
}

#zmzwaouylb .gt_column_spanner_outer {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: normal;
  text-transform: inherit;
  padding-top: 0;
  padding-bottom: 0;
  padding-left: 4px;
  padding-right: 4px;
}

#zmzwaouylb .gt_column_spanner_outer:first-child {
  padding-left: 0;
}

#zmzwaouylb .gt_column_spanner_outer:last-child {
  padding-right: 0;
}

#zmzwaouylb .gt_column_spanner {
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: bottom;
  padding-top: 5px;
  padding-bottom: 5px;
  overflow-x: hidden;
  display: inline-block;
  width: 100%;
}

#zmzwaouylb .gt_group_heading {
  padding: 8px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
}

#zmzwaouylb .gt_empty_group_heading {
  padding: 0.5px;
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  vertical-align: middle;
}

#zmzwaouylb .gt_from_md > :first-child {
  margin-top: 0;
}

#zmzwaouylb .gt_from_md > :last-child {
  margin-bottom: 0;
}

#zmzwaouylb .gt_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  margin: 10px;
  border-top-style: solid;
  border-top-width: 1px;
  border-top-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 1px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 1px;
  border-right-color: #D3D3D3;
  vertical-align: middle;
  overflow-x: hidden;
}

#zmzwaouylb .gt_stub {
  color: #333333;
  background-color: #FFFFFF;
  font-size: 100%;
  font-weight: initial;
  text-transform: inherit;
  border-right-style: solid;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
  padding-left: 12px;
}

#zmzwaouylb .gt_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#zmzwaouylb .gt_first_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
}

#zmzwaouylb .gt_grand_summary_row {
  color: #333333;
  background-color: #FFFFFF;
  text-transform: inherit;
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
}

#zmzwaouylb .gt_first_grand_summary_row {
  padding-top: 8px;
  padding-bottom: 8px;
  padding-left: 5px;
  padding-right: 5px;
  border-top-style: double;
  border-top-width: 6px;
  border-top-color: #D3D3D3;
}

#zmzwaouylb .gt_striped {
  background-color: rgba(128, 128, 128, 0.05);
}

#zmzwaouylb .gt_table_body {
  border-top-style: solid;
  border-top-width: 2px;
  border-top-color: #D3D3D3;
  border-bottom-style: solid;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
}

#zmzwaouylb .gt_footnotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#zmzwaouylb .gt_footnote {
  margin: 0px;
  font-size: 90%;
  padding: 4px;
}

#zmzwaouylb .gt_sourcenotes {
  color: #333333;
  background-color: #FFFFFF;
  border-bottom-style: none;
  border-bottom-width: 2px;
  border-bottom-color: #D3D3D3;
  border-left-style: none;
  border-left-width: 2px;
  border-left-color: #D3D3D3;
  border-right-style: none;
  border-right-width: 2px;
  border-right-color: #D3D3D3;
}

#zmzwaouylb .gt_sourcenote {
  font-size: 90%;
  padding: 4px;
}

#zmzwaouylb .gt_left {
  text-align: left;
}

#zmzwaouylb .gt_center {
  text-align: center;
}

#zmzwaouylb .gt_right {
  text-align: right;
  font-variant-numeric: tabular-nums;
}

#zmzwaouylb .gt_font_normal {
  font-weight: normal;
}

#zmzwaouylb .gt_font_bold {
  font-weight: bold;
}

#zmzwaouylb .gt_font_italic {
  font-style: italic;
}

#zmzwaouylb .gt_super {
  font-size: 65%;
}

#zmzwaouylb .gt_footnote_marks {
  font-style: italic;
  font-weight: normal;
  font-size: 65%;
}
</style>
<table class="gt_table">
  <thead class="gt_header">
    <tr>
      <th colspan="2" class="gt_heading gt_title gt_font_normal gt_bottom_border" style>Таблица 9. Изчисляване на стандартизираните показатели</th>
    </tr>
    
  </thead>
  <thead class="gt_col_headings">
    <tr>
      <th class="gt_col_heading gt_columns_bottom_border gt_center" rowspan="1" colspan="1">group</th>
      <th class="gt_col_heading gt_columns_bottom_border gt_right" rowspan="1" colspan="1">total_fatality_rate_standardized</th>
    </tr>
  </thead>
  <tbody class="gt_table_body">
    <tr><td class="gt_row gt_center">unvaccinated</td>
<td class="gt_row gt_right">81.25</td></tr>
    <tr><td class="gt_row gt_center">vaccinated</td>
<td class="gt_row gt_right">71.25</td></tr>
  </tbody>
  
  
</table>
</div>

Отново стандартизираните показател в групата на ваксинираните с 10%
по-нисък от този на неваксинираните.
