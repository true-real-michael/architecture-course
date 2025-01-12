
# Bookstore

![bookstore/bookstore.svg](bookstore.svg)

# Выполнили
1. [Киселёв Михаил, 21.Б07-мм](https://github.com/true-real-michael)
2. [Громова Арабелла, 21.Б10-мм](https://github.com/rongirl)
3. [Житнухина Мария, 21.Б10-мм](https://github.com/zhitm)

## Модули и классы

1. `Catalog`:
    1. `Book` --- класс книги
    2. `SellItem` --- класс страницы товара в интернет магазине. Разные продавцы могут продавать одну книгу на разных страницах товара. 
    3. `Catalog` --- класс, отвечающий за получение и фильтрацию книг.
    4. `FilterSpec` --- спецификация для фильтрации с помощью `Catalog`.
    5. `CatalogRenderer` --- создает мини-каталог в соответствии с переданной ему `FilterSpec`.
    6. `Review`, `ModeratorReview`, `UserReview` --- отзывы.
2. `Users`:
    1. `AuthService` --- если ему передали правильные данные для входа, возвращает пользователя.
    2. `User` --- абстрактный класс пользователя.
    3. `Moderator` --- модератор, может оставлять модераторские отзывы, ревьюить отзывы покупателей.
    4. `Customer` --- покупатель. Имеет список желаемых товаров `Wishlist` и корзину `ShoppingCart`. Может создавать `Order`.
3. `Orders`
    1. `Order` --- заказ. Имеет `OrderState` и `PaymentMethod`, может иметь или не иметь `Refund`.
    2. `OrderState`, `RefundState` --- состояния заказа и возврата.
    3. `PaymentMethod` --- способ оплаты.
