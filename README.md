# php-api-client

 $factomosApi = new Factomos([
                'FACTOMOS_API_DOMAIN' => FACTOMOS_API_DOMAIN,
                'FACTOMOS_API_VERSION' => FACTOMOS_API_VERSION,
                'FACTOMOS_API_TOKEN' => FACTOMOS_API_TOKEN
                ]);
                
                
$invoice = $factomosApi->createInvoice([
                "document_title" => "Ma Facture",
                "contact_pid" => 456,
                "client_company_name" => 'Nom du client',
                "client_full_address" => '5 Rue de la Terrasse 75017 Paris,
                "subject" => 'Mon objet,
                "invoice_attention" => "John Doe",
                "articleList" => [
                    [
                        'article_pid' => "65478e",
                        'description' => 'Mon premier article,
                        'quantity' => 1,
                        'price' => 500,
                    ],
                    [
                        'article_pid' => "8797r",
                        'description' => 'Mon second article,
                        'quantity' => 1,
                        'price' => 150,
                    ],
                 ],
                "invoice_date" => '2017-02-25',
]);                
            