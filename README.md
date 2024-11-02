# 🎃 Desafío de Halloween.dev - Crear una Poción Mágica 🧙‍♀️

<p>Bienvenido al desafío de Halloween.dev, donde ayudaremos a una bruja a combinar sus pociones mágicas para alcanzar un poder específico. ¡Acompáñanos en esta aventura mágica!</p>

---

## 📜 Problema

<p>Dada una lista de enteros, cada uno representando el poder de una poción, y un número entero que representa el poder objetivo, debes encontrar los índices de las dos primeras pociones que sumen exactamente el poder objetivo. Si no hay combinación posible, la función debe devolver <code>undefined</code>.</p>

### Ejemplos

- **Ejemplo 1:**
  ```
  const potions = [4, 5, 6, 2];
  const goal = 8;
  createMagicPotion(potions, goal); // [2, 3]
   ```

- **Ejemplo 2:**

 ``` 
  const potions = [1, 2, 3, 4];
  const goal = 9;
  createMagicPotion(potions, goal); // undefined
 ```

- **Ejemplo 3:**
   
    ```
    const potions = [1, 2, 3, 4];
    const goal = 5;
    createMagicPotion(potions, goal); // [1, 2]
    ```

    
📋 Requisitos

<ul> <li>Seleccionar la combinación cuya segunda poción aparezca primero en la lista si hay múltiples combinaciones posibles.</li> <li>Devolver <code>undefined</code> si no hay combinación que sume al poder objetivo.</li> </ul>


💻 Implementación

<p>A continuación, se presenta una posible implementación de la función <code>createMagicPotion</code>:</p>

 ```
function createMagicPotion(potions, goal) {
    for (let i = 0; i < potions.length; i++) {
        for (let j = i + 1; j < potions.length; j++) {
            if (potions[i] + potions[j] === goal) {
                return [i, j];
            }
        }
    }
    return undefined;
}
 ```
🚀 Cómo Ejecutar el Proyecto

<ol> <li>Asegúrate de tener <a href="https://nodejs.org/" target="_blank">Node.js</a> instalado en tu máquina.</li> <li>Clona este repositorio: <pre><code>git clone https://github.com/tuusuario/nombre-del-repositorio.git</code></pre> </li> <li>Navega al directorio del proyecto: <pre><code>cd nombre-del-repositorio</code></pre> </li> <li>Ejecuta el archivo JavaScript: <pre><code>node tuarchivo.js</code></pre> </li> </ol>


