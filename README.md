									# Catálogo de Jogos 🚀

### Neste programa, vamos utilizar o swagger como um banco de dados dos jogos cadastrado. Utilizamos o Visual Studio 2019, o .NET Core e a linguagem C sharp. Neste programa poderemos cadastrar o Jogo, a sua devida produtora, o ano de lançamento, o gênero e o valor deste jogo no mercado. Abaixo, está o programa principal com os seus devidos parâmetros e comandos (as outras class serão adicionada no GitHub):



1. *_Program.cs_:*

   using Microsoft.AspNetCore.Hosting;
   using Microsoft.Extensions.Configuration;
   using Microsoft.Extensions.Hosting;
   using Microsoft.Extensions.Logging;
   using System;
   using System.Collections.Generic;
   using System.Linq;
   using System.Threading.Tasks;

   namespace ApiCatalogosJogos
   {
       public class Program
       {
           public static void Main(string[] args)
           {
               CreateHostBuilder(args).Build().Run();
           }
       
           public static IHostBuilder CreateHostBuilder(string[] args) =>
               Host.CreateDefaultBuilder(args)
                   .ConfigureWebHostDefaults(webBuilder =>
                   {
                       webBuilder.UseStartup<Startup>();
                   });
       }
   }