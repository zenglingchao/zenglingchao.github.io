直接上干货。

1.使用SerializedName注解为参数提供备用名。

```
@SerializedName("email_address")
public String emailAddress;
```

```
@SerializedName(value = "emailAddress", alternate = {"email", "email_address"})
public String emailAddress;
```

注解参数传入单个String 或String数组 ，解析时就能够对相应的参数进行解析。

