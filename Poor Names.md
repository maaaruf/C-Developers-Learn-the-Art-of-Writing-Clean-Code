# Poor Names

## Mysterious Names

Sometimes we use mysterious names to our code, which is not readble by other developer. Even if we came back later we can't understand the identifiers purpose by looking at the name only. So that We should avoid to use that. Some Example of Mysterious Names are

```C#
SqlDataReader dr1
int od

void Button1_Click()

Class Page1{}
```

This names can be more readable like

``` C#
SqlDataReader dataReader
int overdueDays

void CheckAvailability_Click()

Class CustomerPageView{}
```

## Meaningless Names

Names should express a easy meaning always. Writing a big name with no meaning is useless.Like `void BeginCheckFunctionality_StoreClinetSideCheckboxIDsArray();` mehodname is meaningless here. We named it with a big deatil but ultimately it's not meaningful. If we need to understand the meaning then we need to read it's implimentation. Which is not fruitful.

## Names with Encodings

In past people uses hungerian notation to understand the types of a variable like `int iMaxRequest`, As nowdays IDEs are more powerful, these are not needed now. The variable name should be without hungerian notaion like `maxRequest`.

```C#
var m_objCollection = new StringCollection();
```

In this scenario if we look at the name **m_objCollection** is not telling us what is inside it, it's a Mysterious name also. The variable can be named with `countryNames`

## Ambiguous Names

When a name express multiple meaning then we can identify it as Ambigous Names.

```C#
IList<string> DatabaseOperation(){}
string Convert(DateTime date){}
```

These methods are indicating a meaning though but we are not getting clear message by the name. There are many database operations, Which operation is performing the _**DatabaseOperation**_ method? Same thing also happend with _**Convert**_ method. These method names can be more meaningful like

```C#
IList<string> InsertIntoDB(){}
string ConvertToString(DateTime date){}
```

## Noisy Names

Names with unecessary prefix postfix, or lengthy name which is possible to be avoided. Like

```C#
theDateOfBirth     -> birthDate
NumberOfRecord     -> RecordCount
```

## Things to remember to avoid smelly names

* Not too short, not too long
* Meaningful
* Reveal Intension
* Chosen from problem domain
