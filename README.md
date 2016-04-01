# crescente 
  int num1, num2, num3, pri = 0, seg = 0, terc = 0;

            Console.WriteLine("Digite o primeiro numero");
            num1 = Convert.ToInt16(Console.ReadLine());

            Console.WriteLine("Informe o segundo numero");
            num2 = Convert.ToInt16(Console.ReadLine());

            if (num1 > num2)
            {
                pri = num1;
                seg = num2;

            }
            else
            {
                pri = num2;
                seg = num1;
             }
            Console.WriteLine("Informe o terceiro numero");
            num3 = Convert.ToInt16(Console.ReadLine());

            if (num3 > num1 && num3 > num2)
            {
                pri = num3;
                if (num1 > num2)
                {
                    seg = num1;
                    terc = num3;

                }
                else
                {
                    seg = num2;
                    terc = num1;
                }
            }
            else if (num3 > num1 && num3 < num2)
            {
                pri = num2;
                seg = num3;
                terc = num1;

            }
            else
            {
                terc = num3;
            }

            Console.Write("Numeros em ordem crescente: {2}, {1}, {0}", pri, seg, terc);
            Console.Read();
            
            }
