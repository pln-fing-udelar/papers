# NLP papers, tl;dr

## General 

- ⭐ Bender, E. M., & Koller, A. (2020). Climbing towards NLU: On meaning, form, and understanding in the age of data. In Proc. of ACL.
  - Abstract: The success of the large neural language models on many NLP tasks is exciting. However, we find that these successes sometimes lead to hype in which these models are being described as “understanding” language or capturing “meaning”. In this position paper, we argue that a system trained only on form has a priori no way to learn meaning. In keeping with the ACL 2020 theme of “Taking Stock of Where We’ve Been and Where We’re Going”, we argue that a clear understanding of the distinction between form and meaning will help guide the field towards better science around natural language understanding. 
  - tl;dr Comentan que, a partir de la mejora en muchas tareas de NLP luego de los modelos de lenguaje tipo BERT o GPT-2, hay mucho hype, y que mucho viene del hecho de no entender bien la diferencia entre forma lingüística y significado. Todavía no sabemos siquiera bien lo que aprenden los LM. Definen significado y aclaran la diferencia entre intención comunicativa y el significado convencional de una expresión. Presentan un ejemplo maravilloso, que llaman el Octopus test, donde hay dos náufragos en dos islas, que se comunican a través de un cable; un pulpo "pincha" el cable, y empieza a escucharlos. Luego de suficiente tiempo, el pulpo se pone en el medio y responde por uno de ellos. Analizan qué podría hacer en esas condiciones (es parecido a un Turing test, pero no exactamente igual). Proponen otros experimentos interesantes. Más en general, se plantean la pregunta de si "estamos subiendo la colina indicada": si lo vemos bottom-up, una cantidad de tareas se resuelven mejor. La pregunta es si estamos avanzando hacia hacia la comprensión o a pasar el Turing test o a lo que sea nuestro gran objetivo. Proponen algunas buenas prácticas para subir la colina indicada. 
  
## Adversarial Examples

- (2017) R.Jia and P. Liang: [Adversarial Examples for Evaluating Reading Comprehension Systems](https://arxiv.org/abs/1707.07328) 
  - tl;dr: A partir del corpus [SQuAD](https://rajpurkar.github.io/SQuAD-explorer/) (que incluye un párrafo de Wikipedia, una pregunta y sus respuesta), los autores crean ejemplos adversarios agregando una oración adversaria al párrafo (_concatenative adversaries_), que buscan confundir a la pregunta, porque son parecidas (pero no contradicen) a la pregunta y sugieren una respuesta. Hacen caer el F1-score de 75% a 36%. Presentan también un método independiente del modelo, que agrega una oración aleatoria (pero con sentido) al párrafo.

### Otros repositorios

- [nlp-library](https://github.com/mihail911/nlp-library), by [Mihail Erik](https://github.com/mihail911)
