# orm.hibernate Skill

Use this skill to work with Norm module `orm.hibernate` version 5. Use only declarations listed below.

## `orm.hibernate`

Source: `Builder.norm`

### `Builder`

```norm
class Builder
```

#### `Builder`

```norm
Builder(__JarBindingToken token)
```

Parameters:

- `token`: `__JarBindingToken`

#### `addAnnotatedClass`

```norm
Builder? addAnnotatedClass(Class<?>? arg0)
```

Parameters:

- `arg0`: `Class<?>?`

Returns: `Builder?`

#### `buildSessionFactory`

```norm
Provider? buildSessionFactory()
```

Returns: `Provider?`

#### `setProperty`

```norm
Builder? setProperty(String? arg0, String? arg1)
```

Parameters:

- `arg0`: `String?`
- `arg1`: `String?`

Returns: `Builder?`

### `builderNew`

```norm
Builder builderNew()
```

Returns: `Builder`

## `orm.hibernate`

Source: `Provider.norm`

### `Provider`

```norm
interface Provider extends EntityManagerFactory, Serializable
```

#### `close`

```norm
Void close()
```

Returns: `Void`

#### `isOpen`

```norm
Boolean isOpen()
```

Returns: `Boolean`

#### `openSession`

```norm
Session? openSession()
```

Returns: `Session?`

## `orm.hibernate`

Source: `Session.norm`

### `Session`

```norm
interface Session extends SharedSessionContract, EntityManager
```

#### `beginTransaction`

```norm
Transaction? beginTransaction()
```

Returns: `Transaction?`

#### `close`

```norm
Void close()
```

Returns: `Void`

#### `find`

```norm
T? find<T>(Class<T>? arg0, Any? arg1)
```

Type parameters:

- `T`

Parameters:

- `arg0`: `Class<T>?`
- `arg1`: `Any?`

Returns: `T?`

#### `flush`

```norm
Void flush()
```

Returns: `Void`

#### `persist`

```norm
Void persist(Any? arg0)
```

Parameters:

- `arg0`: `Any?`

Returns: `Void`

#### `remove`

```norm
Void remove(Any? arg0)
```

Parameters:

- `arg0`: `Any?`

Returns: `Void`

## `orm.hibernate`

Source: `SharedSessionContract.norm`

### `SharedSessionContract`

```norm
interface SharedSessionContract extends QueryProducer, AutoCloseable, Serializable
```

#### `close`

```norm
Void close()
```

Returns: `Void`

## `orm.hibernate`

Source: `Transaction.norm`

### `Transaction`

```norm
interface Transaction extends EntityTransaction
```

#### `commit`

```norm
Void commit()
```

Returns: `Void`

#### `isActive`

```norm
Boolean isActive()
```

Returns: `Boolean`

#### `rollback`

```norm
Void rollback()
```

Returns: `Void`

## `orm.hibernate.jakarta.persistence`

Source: `jakarta/persistence/EntityManagerFactory.norm`

### `EntityManagerFactory`

```norm
interface EntityManagerFactory extends AutoCloseable
```

#### `close`

```norm
Void close()
```

Returns: `Void`

## `orm.hibernate.jakarta.persistence`

Source: `jakarta/persistence/EntityTransaction.norm`

### `EntityTransaction`

```norm
interface EntityTransaction
```

## `orm.hibernate.query`

Source: `query/QueryProducer.norm`

### `QueryProducer`

```norm
interface QueryProducer
```

