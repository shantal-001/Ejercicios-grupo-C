# Ejercicios-grupo-C
PARTE 2 Ejercicio 1
#include <iostream>
#include <fstream>
using namespace std;

int main() {
    ofstream archivo("datos.txt"); // Crear archivo

    if (!archivo) {
        cout << "Error al crear el archivo" << endl;
        return 1;
    }

    string nombre, ciudad;
    int edad;

    cout << "Ingrese su nombre: ";
    cin >> nombre;

    cout << "Ingrese su edad: ";
    cin >> edad;

    cout << "Ingrese su ciudad: ";
    cin >> ciudad;

    archivo << nombre << " " << edad << " " << ciudad << endl;

    archivo.close();

    cout << "Datos guardados correctamente en datos.txt" << endl;

    return 0;
}