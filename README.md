# Отчёт о тестировании приложения расчета баллов бонусной программы

## Краткое описание

22/07/2021  было проведено тестирование приложения расчета бонусной программы

На тестирование затрачено: 0.2 часа 

В результате тестирования выявлены следующие дефекты:
[некорректный рассчет баллов при суммировании дробных значений](https://github.com/eavasil/bonus_system/issues/1#issue-950748347).


## Описание процесса тестирования

В качестве тестовых данных использовались следующие данные: 

public class Main {
  public static void main(String[] args) {
    double regularBonus = 0.3;
    double specialBonus = 0.6;
    double totalBonus = regularBonus + specialBonus;
    System.out.println(totalBonus);
  }
}

Тестирование производилось в следующем окружении:
* Windows 10 Домашняя для одного языка 64 bit
* версия Java11 11.0.11
* Visual Studio Code