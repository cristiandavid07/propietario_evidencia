# Evidencia Propietario
## Proceso realizado desde la terminal:


sena@sena-HP-ProBook-445R-G6:~$ pwd
/home/sena
sena@sena-HP-ProBook-445R-G6:~$ cd desarrollo
sena@sena-HP-ProBook-445R-G6:~/desarrollo$ cd myapp
sena@sena-HP-ProBook-445R-G6:~/desarrollo/myapp$ rails g scaffold Propiedad nombre direccion telefono:integer
You don't have net-smtp installed in your application. Please add it to your Gemfile and run bundle install
Running via Spring preloader in process 6208
      invoke  active_record
      create    db/migrate/20221003143754_create_propiedades.rb
      create    app/models/propiedad.rb
      invoke    test_unit
      create      test/models/propiedad_test.rb
      create      test/fixtures/propiedades.yml
      invoke  resource_route
       route    resources :propiedades
      invoke  scaffold_controller
      create    app/controllers/propiedades_controller.rb
      invoke    erb
      create      app/views/propiedades
      create      app/views/propiedades/index.html.erb
      create      app/views/propiedades/edit.html.erb
      create      app/views/propiedades/show.html.erb
      create      app/views/propiedades/new.html.erb
      create      app/views/propiedades/_form.html.erb
      invoke    resource_route
      invoke    test_unit
      create      test/controllers/propiedades_controller_test.rb
      create      test/system/propiedades_test.rb
      invoke    helper
=> "carlos"
irb(main):029:0> p.save
  TRANSACTION (0.1ms)  begin transaction
  Propiedad Update (0.4ms)  UPDATE "propiedades" SET "nombre" = ?, "updated_at" = ? WHERE "propiedades"."id" = ?  [["nombre", "carlos"], ["updated_at", "2022-10-03 14:54:53.126400"], ["id", 2]]                                      
  TRANSACTION (7.6ms)  commit transaction                              
=> true                                                                
irb(main):030:0> Propiedad.all
  Propiedad Load (0.3ms)  SELECT "propiedades".* FROM "propiedades"
=>                                                                   
[#<Propiedad:0x00007f471bdc0528                                      
  id: 1,                                                             
  nombre: "primera",                                                 
  direccion: "k6l1-101",                                             
  telefono: 12345,                                                   
  created_at: Mon, 03 Oct 2022 14:43:32.779156000 UTC +00:00,        
  updated_at: Mon, 03 Oct 2022 14:43:32.779156000 UTC +00:00>,       
 #<Propiedad:0x00007f471bdc0258                                      
  id: 2,                                                             
  nombre: "carlos",                                                  
  direccion: "k6l2-102",                                             
  telefono: 23456,                                                   
=>                                                                     
#<Propiedad:0x00007f471b80d6a8                                         
 nombre: "tercera",                                                    
 direccion: "k6l3-103",                                                
 telefono: 34567,                                            
 created_at: Mon, 03 Oct 2022 14:48:26.212430000 UTC +00:00, 
 updated_at: Mon, 03 Oct 2022 14:48:26.212430000 UTC +00:00> 
irb(main):033:0> Propiedad.all
  Propiedad Load (0.3ms)  SELECT "propiedades".* FROM "propiedades"
=>                                                                   
[#<Propiedad:0x00007f4719f358b0                                      
  id: 1,                                                             
  nombre: "primera",                                                 
  direccion: "k6l1-101",                                             
  telefono: 12345,                                                   
  created_at: Mon, 03 Oct 2022 14:43:32.779156000 UTC +00:00,        
  updated_at: Mon, 03 Oct 2022 14:43:32.779156000 UTC +00:00>,       
 #<Propiedad:0x00007f4719f357e8                                      
  id: 2,
  nombre: "carlos",                                                  
  direccion: "k6l2-102",                                             
  telefono: 23456,                                                   
  created_at: Mon, 03 Oct 2022 14:46:51.708648000 UTC +00:00,        
  updated_at: Mon, 03 Oct 2022 14:54:53.126400000 UTC +00:00>,
 #<Propiedad:0x00007f4719f356f8
  id: 4,
  nombre: "cuarta",
  direccion: "k6l4104",
  telefono: 45678,
  created_at: Mon, 03 Oct 2022 14:50:46.190241000 UTC +00:00,
  updated_at: Mon, 03 Oct 2022 14:50:46.190241000 UTC +00:00>,
 #<Propiedad:0x00007f4719f355e0
  id: 5,
  nombre: "quinta",
  direccion: "k6l5105",
  telefono: 67896,
  created_at: Mon, 03 Oct 2022 14:52:24.148312000 UTC +00:00,
  updated_at: Mon, 03 Oct 2022 14:52:24.148312000 UTC +00:00>]
irb(main):034:0> 
^C
irb(main):034:0>
