# Comments

任何以感叹号开头的行都是注释。在规则列表中，它以灰色显示。 AdGuard 将忽略这一行，因此您可以编写任何您想要的内容。注释通常放置在规则之上，用于描述规则的作用。

## 通过域名屏蔽

![Image text](https://github.com/arqady01/adguard_rules/blob/main/0_blocking_domain.svg)

**This rule blocks:**

- `http://example.org/ad1.gif`
- `http://subdomain.example.org/ad1.gif`
- `https://ads.example.org:8000/`

**This rule does not block:**

- `http://ads.example.org.us/ad1.gif`
- `http://example.com/redirect/http://ads.example.org/`

## 阻止确切地址

![Image text](https://github.com/arqady01/adguard_rules/blob/main/1_exact_address.svg)

**This rule blocks:**

- `http://example.org/`

**This rule does not block:**

- `https://example.org/banner/img`

## 基本规则修改器

![Image text](https://github.com/arqady01/adguard_rules/blob/main/2_basic_rule_options.svg)

过滤规则支持多种修饰符，允许您微调规则行为。下面是带有一些简单修饰符的规则示例。

**This rule blocks:**

- http://example.org/script.js if this script is loaded from example.org.

**This rule does not block:**

- https://example.org/script.js if this script is loaded from example.org.
- https://example.org/banner.png because it is not a script.

