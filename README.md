# templatesCpp
馃捇 - Lecci贸n de Programaci贸n de estructuras de datos y algoritmos fundamentales || Itesm Tercer Semestre

驴Que son los templates?
馃 Definici贸n: El uso de Templates (Plantillas) es una caracter铆stica del lenguaje de programaci贸n C++ en el cual permite que funciones y clases operen con tipos de datos gen茅ricos, permitiendo con esto que una funci贸n o clase trabaje en muchos tipos de datos sin tener que reescribirse para cada uno. 

Ejemplo de funci贸n: 

template <typename T>
T menor(T uno, T dos){
  if (uno < dos){
       return uno;
  }
  return dos;
}

template <class T>                 
class Value{                 
     public:            
          Value();       
          Value(T);    
          T getValue;
          void setValue(T value);
     private:
          T value;
};

template <class T>
Value<T>::Value(T value){
      this->value = value; 
}
  
template <class T>
T Value<T>::getValue(){
      return this->value;
}
