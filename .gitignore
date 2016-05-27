using System;
using System.Collections.Generic;
using System.Linq;
using System.Text;
using System.Threading.Tasks;

namespace ConsoleApplication5
{
    class Program
    {
        static void Main(string[] args)
        {
            for (;;)
            {
                string novotexto = "";
                string caracteres = "!@#$%¨&*()_-+ abcdefghijklmnopqrstuvwxyz";
                Console.WriteLine("Escreva uma frase");
                string texto = Console.ReadLine();
                Console.WriteLine("Escreva a chave");
                int chave = int.Parse(Console.ReadLine());
                Console.WriteLine("Você quer criptografar ou descriptografar?");
                string escolha = Console.ReadLine();

                char[] caractereschar = caracteres.ToCharArray();
                char[] textochar = texto.ToLower().ToCharArray();


                if (escolha.ToLower() == "criptografar")
                {


                    for (int i = 0; i < textochar.Length; i++)
                    {
                        for (int n = 0; n < caractereschar.Length; n++)
                        {
                            if (textochar[i] == caractereschar[n])
                            {
                                if ((n + chave) <= (caractereschar.Length - 1))
                                {
                                    novotexto += caractereschar[n + chave];
                                }
                                else
                                {
                                    novotexto += caractereschar[(n + chave) - (caractereschar.Length)];
                                }
                            }
                        }
                    }
                    Console.WriteLine(novotexto);
                }

                else if (escolha.ToLower() == "descriptografar")
                {
                    for (int i = 0; i < textochar.Length; i++)
                    {
                        for (int n = 0; n < alfabetochar.Length; n++)
                        {
                            if (textochar[i] == alfabetochar[n])
                            {
                                if ((n - chave) >= 0)
                                {
                                    novotexto += alfabetochar[n - chave];
                                }
                                else
                                {
                                    novotexto += alfabetochar[(n - chave) + alfabetochar.Length];
                                }
                            }
                        }
                    }
                    Console.WriteLine(novotexto);
                }
                else
                {
                    Console.WriteLine("Escreva corretamente");
                }

                Console.ReadKey();
                Console.Clear();
            }




        }
        }
        
    }

