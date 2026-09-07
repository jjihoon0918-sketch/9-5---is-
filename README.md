# 9-5---is-

# C# `is` 키워드

`is`는 객체가 **특정 타입인지 확인할 때** 사용하는 키워드이다.

## 특징

- 해당 타입이면 `true`
- 아니면 `false`
- 타입 확인 후 안전하게 사용할 수 있음
- 패턴 매칭으로 형 변환까지 동시에 가능

## 예제

```csharp
Animal animal = new Dog();

if (animal is Dog dog)
{
    dog.Bark();
}
```

`animal`이 `Dog` 타입이면 `dog` 변수로 바로 사용할 수 있다.

## `is`와 `as` 차이

| `is` | `as` |
|---|---|
| 타입 확인 | 형 변환 |
| `true` / `false` 반환 | 실패 시 `null` 반환 |

## 한 줄 정리

> `is` = 객체가 특정 타입인지 확인하는 키워드