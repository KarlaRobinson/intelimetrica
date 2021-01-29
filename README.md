# Intelimetrica
# startup Melp
# App para brindar información sobre los mejores restaurantes de la ciudad.


class CreateRestaurantes < ActiveRecord::Migration[5.0]
  def change
    create_table :restaurantes do |t|
      t.integer :rating -- Numero de 0 a 4
      t.string :name -- Nombre del restaurante
      t.string :site -- Sitio de Web
      t.string :email -- Email
      t.string :phone -- Telefono
      t.string :street -- Calle
      t.string :city -- Ciudad
      t.string :state -- Estado
      t.string :lat -- Latitud
      t.string :lng -- Longitud
      t.timestamps
    end
  end
end
