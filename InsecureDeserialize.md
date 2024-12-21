

# What is serialization?
- Serialization is the proccess of converting complex data structures, such as objects and their fields , into a "flatter" format that can be sent and received as a sequential stream of bytes.
- When serializing an object, its state is also persisted. In ther words, the object's attributes are preserved, along with their assigned values

## Serialization vs deserialization
- Deserialization is the process of restoring this byte stream to a fully functional replica of the original object, in the exact state as when it was serialized.
- "serialization" ~ marshalling (Ruby) ~ pickling (Python)

# What is insecure deserialization?
update soon 



# How do insecure deserialization vulnerabilities  arise?
update soon 

# What is the impact of insecure deserializaition? 
update soon 

# Exploit

## Identify insecure deserialization

### PHP serialization format
```txt
O:4:"User":2:{s:4:"name":s:6:"carlos"; s:10:"isLoggedIn":b:1;}
```
### Java serialization format
- Some languages includes Java, use binary serialization formats, can be recognized by few tell-tale signs.
- serialized Java objects always begin with the same bytes (ex: ro0 in base64)

## Manipulating serialized objects
- Edit the object directly in its byte stream form
- Write a short script in the corresponding programming language to create and serialize the new object.

### Modifing object attributes
### Modifying data types

## Using application functionality
- Attacker can use insecure deserialization to pass in unexpected data and leverage the related functionality to do damage

## Magic methods
- Magic methods are a special subset of methods that invoked automatically whenever a particular event or scenario occurs instead of invoked explicitly


## Inject arbitrary objects


## Gadget chains

### Pre-built gadget chains
1. ysoserial
2. PHP Generic Gadget Chains

### Documented gadget chains
update soon 
## Creating your own exploit
update soon 
## PHAR deserialization


