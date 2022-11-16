Team Members :
1. Alfitra Fadjri (1313620027)
2. Fozan Bebe Moreno (1313620041)
3. Zhafran Panggomgomi (1313620020)

#### Untuk android studio versi lama, apabila terdapat error berikut : 
```
"Inheritance from an interface with '@JvmDefault' members is only allowed with -Xjvm-default option"
```
**Tambahkan baris code berikit pada gradle.app :**

```
android {

   ...
   kotlinOptions {
   
       ...
       freeCompilerArgs += [
                "-Xjvm-default=all",
        ]
   }
}
```
