# Отчёт о тестировании <Credit Card Number Validator>
## Краткое описание
09.08.2021 - 10.08.2021 было проведено функциональное тестирование валидаций банковских карт.

На тестирование затрачено: 24 часа

В результате тестирования выявлены следующие дефекты:

* [Ошибка при проверке номеров банковских карт American Express (AMEX)](https://github.com/Anvar102rus/Bank-card-testing-report/issues/2#issue-965066572)
* [Ошибка при тестировании номеров банковских карт Diners Club - Carte Blanche](https://github.com/Anvar102rus/Bank-card-testing-report/issues/3#issue-965078960)
* [Ошибка при тестировании номеров банковских карт JCB](https://github.com/Anvar102rus/Bank-card-testing-report/issues/4#issue-965086821)
* [Ошибка при тестировании номеров банковских карт VISA](https://github.com/Anvar102rus/Bank-card-testing-report/issues/5#issue-965092595)

## Описание процесса тестирования
 В процессе тестирования использовались следующие артефакты*:

* Процессе тестирования не использовались артефакты тестирования

В качестве тестовых данных использовались данные <https://www.freeformatter.com/credit-card-number-generator-validator.html>:

* American Express (AMEX): 

346819110569015 - FAIL

348448781085354 - FAIL

373665626559990 - FAIL
* Diners Club - Carte Blanche:

30045795676146 - FAIL

30168125524925 - FAIL

30203970063388 - FAIL
* InstaPayment:

6398008547012203 - OK

6376349833092962 - OK

6383994076305869 - OK
* JCB:

3589384732737599 - OK

3534677175308174 - OK

3533598893676247730 - FAIL
* Maestro:

6761847420014631 - OK

6304323641493586 - OK

0604883984624675 - OK
* MasterCard:

2720991061836347 - OK

5209072966019405 - OK

2720996995881285 - OK
* VISA:

4929640997487585 - OK

4532131660793128 - OK

4556109262073712989 - FAIL

Тестирование производилось в следующем окружении:

* Windows 10 Pro и 32-разрядная операционная система, процессор x64
* openjdk version "11.0.11" 2021-04-20
OpenJDK Runtime Environment AdoptOpenJDK-11.0.11+9 (build 11.0.11+9)
OpenJDK Client VM AdoptOpenJDK-11.0.11+9 (build 11.0.11+9, mixed mode)
* IntelliJ IDEA 2020.1