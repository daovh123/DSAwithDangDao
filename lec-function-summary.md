# Tóm tắt các hàm Python được sử dụng trong thư mục `lec`

| Hàm | Dùng để làm gì | Cách dùng | Ví dụ |
|---|---|---|---|
| `Table` | Tạo bảng dữ liệu Table. | `Table(make_array('First Card', 'Second Card'))` | `Table(make_array('First Card', 'Second Card'))` |
| `Table.interactive_plots` | Bật chế độ hiển thị đồ họa tương tác. | `Table.interactive_plots()` | `Table.interactive_plots()` |
| `Table.read_table` | Đọc dữ liệu từ CSV/URL vào Table. | `Table.read_table('farmers_markets.csv')` | `Table.read_table('farmers_markets.csv')` |
| `Table.static_plots` | Bật chế độ hiển thị đồ họa tĩnh. | `Table.static_plots()` | `Table.static_plots()` |
| `a_sample.column` | Lấy cột dữ liệu từ Table. | `a_sample.column('Total Compensation')` | `a_sample.column('Total Compensation')` |
| `a_sample.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `a_sample.hist('Total Compensation', bins = np.arange(0, 800000, 25000))` | `a_sample.hist('Total Compensation', bins = np.arange(0, 800000, 25000))` |
| `a_sample.sample` | Lấy mẫu ngẫu nhiên từ Table. | `a_sample.sample(k = a_sample.num_rows, with_replacement = True)` | `a_sample.sample(k = a_sample.num_rows, with_replacement = True)` |
| `abs` | Lấy giá trị tuyệt đối. | `abs(means_array.item(1)-means_array.item(0))` | `abs(means_array.item(1)-means_array.item(0))` |
| `actors.plot` | Vẽ biểu đồ từ Table dữ liệu. | `actors.plot('Number of Movies', 'Total Gross')` | `actors.plot('Number of Movies', 'Total Gross')` |
| `actors.scatter` | Vẽ biểu đồ phân tán từ Table. | `actors.scatter('Number of Movies', 'Total Gross')` | `actors.scatter('Number of Movies', 'Total Gross')` |
| `actors.where` | Lọc dòng theo điều kiện. | `actors.where('Average per Movie', are.above(400))` | `actors.where('Average per Movie', are.above(400))` |
| `add_subplot` | Hàm Python hoặc method được sử dụng trong notebook. | `plt.figure(figsize=(8,8)).add_subplot(111, projection='3d')` | `plt.figure(figsize=(8,8)).add_subplot(111, projection='3d')` |
| `alice.item` | Lấy giá trị đơn trong hàng/array. | `alice.item(0)` | `alice.item(0)` |
| `all_distances` | Hàm tự định nghĩa trong notebook. | `all_distances(ckd.drop('Class'), alice)` | `all_distances(ckd.drop('Class'), alice)` |
| `all_sales.where` | Lọc dòng theo điều kiện. | `all_sales.where('Bldg Type', '1Fam')` | `all_sales.where('Bldg Type', '1Fam')` |
| `apply` | Hàm Python hoặc method được sử dụng trong notebook. | `test.drop('SalePrice').apply(nn_5_regression_estimate)` | `test.drop('SalePrice').apply(nn_5_regression_estimate)` |
| `are.above` | Phương thức của đối tượng trong notebook. | `are.above(0)` | `are.above(0)` |
| `are.below` | Phương thức của đối tượng trong notebook. | `are.below(999)` | `are.below(999)` |
| `are.between` | Phương thức của đối tượng trong notebook. | `are.between(x_val - 1/2, x_val + 1/2)` | `are.between(x_val - 1/2, x_val + 1/2)` |
| `are.contained_in` | Phương thức của đối tượng trong notebook. | `are.contained_in(make_array('San Francisco', 'New York', 'Chicago'))` | `are.contained_in(make_array('San Francisco', 'New York', 'Chicago'))` |
| `are.equal_to` | Phương thức của đối tượng trong notebook. | `are.equal_to('5')` | `are.equal_to('5')` |
| `are.not_equal_to` | Phương thức của đối tượng trong notebook. | `are.not_equal_to(999)` | `are.not_equal_to(999)` |
| `attributes.apply` | Phương thức của đối tượng trong notebook. | `attributes.apply(distance_from_new_row)` | `attributes.apply(distance_from_new_row)` |
| `averages_tbl.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `averages_tbl.hist(bins = 20)` | `averages_tbl.hist(bins = 20)` |
| `averages_tbl.sort` | Sắp xếp bảng theo cột. | `averages_tbl.sort(0)` | `averages_tbl.sort(0)` |
| `ax.scatter` | Vẽ biểu đồ phân tán từ Table. | `ax.scatter(banknotes.column('WaveletSkew'), 
           banknotes.column('WaveletVar'), 
           banknotes.column('WaveletCurt'), 
           c=banknotes.column('Class'))` | `ax.scatter(banknotes.column('WaveletSkew'), 
           banknotes.column('WaveletVar'), 
           banknotes.column('WaveletCurt'), 
           c=banknotes.column('Class'))` |
| `back_pain.group` | Nhóm dữ liệu theo giá trị cột. | `back_pain.group('Group')` | `back_pain.group('Group')` |
| `back_pain.pivot` | Biến đổi bảng theo hàng/cột. | `back_pain.pivot('Result', 'Group')` | `back_pain.pivot('Result', 'Group')` |
| `back_pain.sample` | Lấy mẫu ngẫu nhiên từ Table. | `back_pain.sample(5, with_replacement = False)` | `back_pain.sample(5, with_replacement = False)` |
| `banknotes.column` | Lấy cột dữ liệu từ Table. | `banknotes.column('WaveletVar')` | `banknotes.column('WaveletVar')` |
| `banknotes.drop` | Xóa cột khỏi Table. | `banknotes.drop('Class')` | `banknotes.drop('Class')` |
| `banknotes.group` | Nhóm dữ liệu theo giá trị cột. | `banknotes.group('Class')` | `banknotes.group('Class')` |
| `banknotes.sample` | Lấy mẫu ngẫu nhiên từ Table. | `banknotes.sample(with_replacement=False)` | `banknotes.sample(with_replacement=False)` |
| `banknotes.scatter` | Vẽ biểu đồ phân tán từ Table. | `banknotes.scatter('WaveletVar', 'WaveletCurt', group='Class')` | `banknotes.scatter('WaveletVar', 'WaveletCurt', group='Class')` |
| `banknotes.split` | Phương thức của đối tượng trong notebook. | `banknotes.split(k = round(banknotes.num_rows/2))` | `banknotes.split(k = round(banknotes.num_rows/2))` |
| `banknotes.take` | Lấy các hàng chỉ định theo chỉ số. | `banknotes.take(np.arange(3))` | `banknotes.take(np.arange(3))` |
| `barh` | Vẽ biểu đồ thanh ngang. | `top_movies.group('Studio').barh('Studio')` | `top_movies.group('Studio').barh('Studio')` |
| `best_line.item` | Lấy giá trị đơn trong hàng/array. | `best_line.item(0)` | `best_line.item(0)` |
| `best_quad.item` | Lấy giá trị đơn trong hàng/array. | `best_quad.item(0)` | `best_quad.item(0)` |
| `binned_data.column` | Lấy cột dữ liệu từ Table. | `binned_data.column('bin')` | `binned_data.column('bin')` |
| `binned_data.show` | Hiển thị nội dung Table. | `binned_data.show()` | `binned_data.show()` |
| `binned_data.take` | Lấy các hàng chỉ định theo chỉ số. | `binned_data.take(np.arange(binned_data.num_rows - 1))` | `binned_data.take(np.arange(binned_data.num_rows - 1))` |
| `binned_data.where` | Lọc dòng theo điều kiện. | `binned_data.where('bin', 40)` | `binned_data.where('bin', 40)` |
| `binned_data.with_column` | Thêm cột mới vào Table. | `binned_data.with_column('Percent', 100*binned_data.column('Age count')/top_movies.num_rows)` | `binned_data.with_column('Percent', 100*binned_data.column('Age count')/top_movies.num_rows)` |
| `births.column` | Lấy cột dữ liệu từ Table. | `births.column('Maternal Pregnancy Weight')` | `births.column('Maternal Pregnancy Weight')` |
| `births.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `births.hist('Maternal Height', bins = np.arange(56.5, 72.6, 1))` | `births.hist('Maternal Height', bins = np.arange(56.5, 72.6, 1))` |
| `births.sample` | Lấy mẫu ngẫu nhiên từ Table. | `births.sample()` | `births.sample()` |
| `births.scatter` | Vẽ biểu đồ phân tán từ Table. | `births.scatter('Gestational Days', 'Birth Weight')` | `births.scatter('Gestational Days', 'Birth Weight')` |
| `births.select` | Chọn cột cần làm việc trong Table. | `births.select('Maternal Smoker')` | `births.select('Maternal Smoker')` |
| `births.show` | Hiển thị nội dung Table. | `births.show(6)` | `births.show(6)` |
| `births.where` | Lọc dòng theo điều kiện. | `births.where('Birth Weight', are.between(birth_weight_mean - birth_weight_sd,
                                        birth_weight_mean + birth_weight_sd))` | `births.where('Birth Weight', are.between(birth_weight_mean - birth_weight_sd,
                                        birth_weight_mean + birth_weight_sd))` |
| `bootstrap_confidence_interval` | Hàm tự định nghĩa trong notebook. | `bootstrap_confidence_interval(original_sample,'Total Compensation', np.max, 95)` | `bootstrap_confidence_interval(original_sample,'Total Compensation', np.max, 95)` |
| `bootstrap_prediction` | Hàm tự định nghĩa trong notebook. | `bootstrap_prediction(births, 'Gestational Days', 'Birth Weight', 230)` | `bootstrap_prediction(births, 'Gestational Days', 'Birth Weight', 230)` |
| `bootstrap_sample.column` | Lấy cột dữ liệu từ Table. | `bootstrap_sample.column('Total Compensation')` | `bootstrap_sample.column('Total Compensation')` |
| `bootstrap_sample.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `bootstrap_sample.hist('Total Compensation', bins = np.arange(0, 800000, 25000))` | `bootstrap_sample.hist('Total Compensation', bins = np.arange(0, 800000, 25000))` |
| `bootstrap_slope_interval` | Hàm tự định nghĩa trong notebook. | `bootstrap_slope_interval(births, 'Gestational Days', 'Birth Weight')` | `bootstrap_slope_interval(births, 'Gestational Days', 'Birth Weight')` |
| `bootstrapped_median_table.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `bootstrapped_median_table.hist(bins = np.arange(125000, 150000, 2000))` | `bootstrapped_median_table.hist(bins = np.arange(125000, 150000, 2000))` |
| `bootstrapped_statistics` | Hàm tự định nghĩa trong notebook. | `bootstrapped_statistics(original_sample,variable,quantity_function)` | `bootstrapped_statistics(original_sample,variable,quantity_function)` |
| `both.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `both.hist('Age in Standard Units', bins = np.arange(-2.2, 3.4, 0.35))` | `both.hist('Age in Standard Units', bins = np.arange(-2.2, 3.4, 0.35))` |
| `career.drop` | Xóa cột khỏi Table. | `career.drop('Semester')` | `career.drop('Semester')` |
| `chebyshev` | Hàm tự định nghĩa trong notebook. | `chebyshev(3)` | `chebyshev(3)` |
| `ckd.column` | Lấy cột dữ liệu từ Table. | `ckd.column('Hemoglobin')` | `ckd.column('Hemoglobin')` |
| `ckd.drop` | Xóa cột khỏi Table. | `ckd.drop('Class')` | `ckd.drop('Class')` |
| `ckd.group` | Nhóm dữ liệu theo giá trị cột. | `ckd.group('Class')` | `ckd.group('Class')` |
| `ckd.join` | Nối hai Table theo khóa chung. | `ckd.join('Class', color_table)` | `ckd.join('Class', color_table)` |
| `ckd.row` | Truy cập hàng trong Table hoặc tạo hàng mới. | `ckd.row(0)` | `ckd.row(0)` |
| `ckd.sample` | Lấy mẫu ngẫu nhiên từ Table. | `ckd.sample(with_replacement=False)` | `ckd.sample(with_replacement=False)` |
| `ckd.scatter` | Vẽ biểu đồ phân tán từ Table. | `ckd.scatter('Hemoglobin', 'Glucose', group='Class')` | `ckd.scatter('Hemoglobin', 'Glucose', group='Class')` |
| `ckd.select` | Chọn cột cần làm việc trong Table. | `ckd.select('Hemoglobin', 'Glucose', 'Class')` | `ckd.select('Hemoglobin', 'Glucose', 'Class')` |
| `ckd.split` | Phương thức của đối tượng trong notebook. | `ckd.split(k = round(ckd.num_rows/2))` | `ckd.split(k = round(ckd.num_rows/2))` |
| `ckd.where` | Lọc dòng theo điều kiện. | `ckd.where('Class',are.equal_to(0))` | `ckd.where('Class',are.equal_to(0))` |
| `ckd.with_column` | Thêm cột mới vào Table. | `ckd.with_column('Distance from Alice', distances)` | `ckd.with_column('Distance from Alice', distances)` |
| `ckd_results.column` | Lấy cột dữ liệu từ Table. | `ckd_results.column('Actual')` | `ckd_results.column('Actual')` |
| `ckd_test.column` | Lấy cột dữ liệu từ Table. | `ckd_test.column('Hemoglobin')` | `ckd_test.column('Hemoglobin')` |
| `ckd_test.select` | Chọn cột cần làm việc trong Table. | `ckd_test.select('Class')` | `ckd_test.select('Class')` |
| `ckd_train.column` | Lấy cột dữ liệu từ Table. | `ckd_train.column('Hemoglobin')` | `ckd_train.column('Hemoglobin')` |
| `ckd_train.select` | Chọn cột cần làm việc trong Table. | `ckd_train.select('Class')` | `ckd_train.select('Class')` |
| `ckd_with_distances.sort` | Sắp xếp bảng theo cột. | `ckd_with_distances.sort('Distance')` | `ckd_with_distances.sort('Distance')` |
| `classify` | Hàm tự định nghĩa trong notebook. | `classify(training=training,p=first_testing_banknote,k=5)` | `classify(training=training,p=first_testing_banknote,k=5)` |
| `classify_grid` | Hàm tự định nghĩa trong notebook. | `classify_grid(ckd.drop('White Blood Cell Count', 'Color'), test_grid, 1)` | `classify_grid(ckd.drop('White Blood Cell Count', 'Color'), test_grid, 1)` |
| `classify_manually` | Hàm tự định nghĩa trong notebook. | `classify_manually(10, 300)` | `classify_manually(10, 300)` |
| `close_points.column` | Lấy cột dữ liệu từ Table. | `close_points.column('Child')` | `close_points.column('Child')` |
| `closest` | Hàm tự định nghĩa trong notebook. | `closest(training, p, k)` | `closest(training, p, k)` |
| `closestk.select` | Chọn cột cần làm việc trong Table. | `closestk.select('Class')` | `closestk.select('Class')` |
| `column` | Lấy cột dữ liệu từ Table. | `simulated_births.group('Shuffled Maternal Smoker',np.average).column(1)` | `simulated_births.group('Shuffled Maternal Smoker',np.average).column(1)` |
| `cone_average_price_table.barh` | Vẽ biểu đồ thanh ngang. | `cone_average_price_table.barh('Flavor')` | `cone_average_price_table.barh('Flavor')` |
| `cones.drop` | Xóa cột khỏi Table. | `cones.drop('Color')` | `cones.drop('Color')` |
| `cones.group` | Nhóm dữ liệu theo giá trị cột. | `cones.group(['Flavor','Color'])` | `cones.group(['Flavor','Color'])` |
| `cones.pivot` | Biến đổi bảng theo hàng/cột. | `cones.pivot('Flavor','Color','Price',np.average)` | `cones.pivot('Flavor','Color','Price',np.average)` |
| `cones.select` | Chọn cột cần làm việc trong Table. | `cones.select('Flavor')` | `cones.select('Flavor')` |
| `cones.show` | Hiển thị nội dung Table. | `cones.show(3)` | `cones.show(3)` |
| `cones.sort` | Sắp xếp bảng theo cột. | `cones.sort('Price')` | `cones.sort('Price')` |
| `cones.where` | Lọc dòng theo điều kiện. | `cones.where('Flavor', 'chocolate')` | `cones.where('Flavor', 'chocolate')` |
| `cones_pivot_table.barh` | Vẽ biểu đồ thanh ngang. | `cones_pivot_table.barh('Color')` | `cones_pivot_table.barh('Color')` |
| `cones_without_color.group` | Nhóm dữ liệu theo giá trị cột. | `cones_without_color.group('Flavor', np.average)` | `cones_without_color.group('Flavor', np.average)` |
| `confidence_interval_95_display` | Hàm tự định nghĩa trong notebook. | `confidence_interval_95_display(100)` | `confidence_interval_95_display(100)` |
| `confidence_interval_sample_30_display` | Hàm tự định nghĩa trong notebook. | `confidence_interval_sample_30_display(n)` | `confidence_interval_sample_30_display(n)` |
| `correlation` | Hàm tự định nghĩa trong notebook. | `correlation(heights, 'Parent Average', 'Child')` | `correlation(heights, 'Parent Average', 'Child')` |
| `counts.column` | Lấy cột dữ liệu từ Table. | `counts.column("Jo")` | `counts.column("Jo")` |
| `create_population` | Hàm tự định nghĩa trong notebook. | `create_population(500/1000, 10000)` | `create_population(500/1000, 10000)` |
| `cumulative_table.plot` | Vẽ biểu đồ từ Table dữ liệu. | `cumulative_table.plot(column_for_xticks='Chapter')` | `cumulative_table.plot(column_for_xticks='Chapter')` |
| `data.column` | Lấy cột dữ liệu từ Table. | `data.column('Year Built')` | `data.column('Year Built')` |
| `decode` | Hàm Python hoặc method được sử dụng trong notebook. | `urlopen(url).read().decode()` | `urlopen(url).read().decode()` |
| `demographics.apply` | Phương thức của đối tượng trong notebook. | `demographics.apply(local_average_income, 'College%')` | `demographics.apply(local_average_income, 'College%')` |
| `demographics.column` | Lấy cột dữ liệu từ Table. | `demographics.column('Median Income')` | `demographics.column('Median Income')` |
| `demographics.drop` | Xóa cột khỏi Table. | `demographics.drop(
    'State', 'District', 'Percent voting for Clinton')` | `demographics.drop(
    'State', 'District', 'Percent voting for Clinton')` |
| `demographics.sample` | Lấy mẫu ngẫu nhiên từ Table. | `demographics.sample(6)` | `demographics.sample(6)` |
| `demographics.scatter` | Vẽ biểu đồ phân tán từ Table. | `demographics.scatter('College%', 'Median Income')` | `demographics.scatter('College%', 'Median Income')` |
| `demographics.select` | Chọn cột cần làm việc trong Table. | `demographics.select('College%', 'Median Income')` | `demographics.select('College%', 'Median Income')` |
| `demographics.show` | Hiển thị nội dung Table. | `demographics.show(5)` | `demographics.show(5)` |
| `demographics.where` | Lọc dòng theo điều kiện. | `demographics.where('College%', are.between(college - a_little, 
                                                              college + a_little))` | `demographics.where('College%', are.between(college - a_little, 
                                                              college + a_little))` |
| `demographics.with_column` | Thêm cột mới vào Table. | `demographics.with_column('Error', errors)` | `demographics.with_column('Error', errors)` |
| `demographics_errors` | Hàm tự định nghĩa trong notebook. | `demographics_errors(slope, intercept)` | `demographics_errors(slope, intercept)` |
| `demographics_rmse` | Hàm tự định nghĩa trong notebook. | `demographics_rmse(1500, 20000)` | `demographics_rmse(1500, 20000)` |
| `die.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `die.hist(bins = make_array(1,2,3,4,5,6,7),unit = 'spot')` | `die.hist(bins = make_array(1,2,3,4,5,6,7),unit = 'spot')` |
| `die.sample` | Lấy mẫu ngẫu nhiên từ Table. | `die.sample(k)` | `die.sample(k)` |
| `die_table.group` | Nhóm dữ liệu theo giá trị cột. | `die_table.group('Result')` | `die_table.group('Result')` |
| `die_table.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `die_table.hist('Result', bins = make_array(0,3,5,6,7), unit = 'Spot')` | `die_table.hist('Result', bins = make_array(0,3,5,6,7), unit = 'Spot')` |
| `die_table.sample` | Lấy mẫu ngẫu nhiên từ Table. | `die_table.sample(1)` | `die_table.sample(1)` |
| `discounts.join` | Nối hai Table theo khóa chung. | `discounts.join('Location',drinks,'Cafe')` | `discounts.join('Location',drinks,'Cafe')` |
| `distance` | Hàm tự định nghĩa trong notebook. | `distance(alice, make_array(row))` | `distance(alice, make_array(row))` |
| `distance_from_alice` | Hàm tự định nghĩa trong notebook. | `distance_from_alice(ckd.drop('Class').row(0))` | `distance_from_alice(ckd.drop('Class').row(0))` |
| `draw_and_compare` | Hàm tự định nghĩa trong notebook. | `draw_and_compare(true_slope=2, true_int=-5, sample_size=10)` | `draw_and_compare(true_slope=2, true_int=-5, sample_size=10)` |
| `draw_line` | Hàm tự định nghĩa trong notebook. | `draw_line(slope=1, intercept=0, color='red')` | `draw_line(slope=1, intercept=0, color='red')` |
| `draw_vertical_line` | Hàm tự định nghĩa trong notebook. | `draw_vertical_line(1.5)` | `draw_vertical_line(1.5)` |
| `drinks.join` | Nối hai Table theo khóa chung. | `drinks.join('Cafe',discounts,'Location')` | `drinks.join('Cafe',discounts,'Location')` |
| `drop` | Xóa cột khỏi Table. | `Table.read_table('breast-cancer.csv').drop('ID')` | `Table.read_table('breast-cancer.csv').drop('ID')` |
| `du_bois.column` | Lấy cột dữ liệu từ Table. | `du_bois.column('ACTUAL AVERAGE')` | `du_bois.column('ACTUAL AVERAGE')` |
| `du_bois.sort` | Sắp xếp bảng theo cột. | `du_bois.sort('ACTUAL AVERAGE', descending=True)` | `du_bois.sort('ACTUAL AVERAGE', descending=True)` |
| `du_bois.where` | Lọc dòng theo điều kiện. | `du_bois.where('ACTUAL AVERAGE', are.above(900))` | `du_bois.where('ACTUAL AVERAGE', are.above(900))` |
| `du_bois.with_column` | Thêm cột mới vào Table. | `du_bois.with_column('FOOD ESTIMATE', food_estimate)` | `du_bois.with_column('FOOD ESTIMATE', food_estimate)` |
| `dugong.scatter` | Vẽ biểu đồ phân tán từ Table. | `dugong.scatter('Length', 'Age')` | `dugong.scatter('Length', 'Age')` |
| `dugong.show` | Hiển thị nội dung Table. | `dugong.show(5)` | `dugong.show(5)` |
| `empirical_distribution` | Hàm tự định nghĩa trong notebook. | `empirical_distribution(100)` | `empirical_distribution(100)` |
| `example.apply` | Phương thức của đối tượng trong notebook. | `example.apply(nn_prediction_example, 'x')` | `example.apply(nn_prediction_example, 'x')` |
| `example.scatter` | Vẽ biểu đồ phân tán từ Table. | `example.scatter('x', 'y')` | `example.scatter('x', 'y')` |
| `example.where` | Lọc dòng theo điều kiện. | `example.where('x', are.between(x_val - 1/2, x_val + 1/2))` | `example.where('x', are.between(x_val - 1/2, x_val + 1/2))` |
| `example.with_column` | Thêm cột mới vào Table. | `example.with_column('Predicted y', example.apply(nn_prediction_example, 'x'))` | `example.with_column('Predicted y', example.apply(nn_prediction_example, 'x'))` |
| `example.with_columns` | Thêm nhiều cột mới vào Table. | `example.with_columns(
    'Predicted y', 
    example.apply(nn_prediction_example, 'x'))` | `example.with_columns(
    'Predicted y', 
    example.apply(nn_prediction_example, 'x'))` |
| `fam.apply` | Phương thức của đối tượng trong notebook. | `fam.apply(name_and_age, 'First Name', 'Birth Year')` | `fam.apply(name_and_age, 'First Name', 'Birth Year')` |
| `fam.with_columns` | Thêm nhiều cột mới vào Table. | `fam.with_columns("Statement",
                 fam.apply(name_and_age, 'First Name', 'Birth Year'))` | `fam.with_columns("Statement",
                 fam.apply(name_and_age, 'First Name', 'Birth Year'))` |
| `families.column` | Lấy cột dữ liệu từ Table. | `families.column('child')` | `families.column('child')` |
| `families.sort` | Sắp xếp bảng theo cột. | `families.sort('family', descending=True)` | `families.sort('family', descending=True)` |
| `families.where` | Lọc dòng theo điều kiện. | `families.where('family', are.equal_to('5'))` | `families.where('family', are.equal_to('5'))` |
| `family_heights.column` | Lấy cột dữ liệu từ Table. | `family_heights.column('mother')` | `family_heights.column('mother')` |
| `family_heights.where` | Lọc dòng theo điều kiện. | `family_heights.where('family', '1')` | `family_heights.where('family', '1')` |
| `farmers_markets.group` | Nhóm dữ liệu theo giá trị cột. | `farmers_markets.group(['Bakedgoods','Vegetables','Seafood'])` | `farmers_markets.group(['Bakedgoods','Vegetables','Seafood'])` |
| `females.column` | Lấy cột dữ liệu từ Table. | `females.column('AGE')` | `females.column('AGE')` |
| `females.show` | Hiển thị nội dung Table. | `females.show(3)` | `females.show(3)` |
| `females_all_rows.where` | Lọc dòng theo điều kiện. | `females_all_rows.where('AGE', are.not_equal_to(999))` | `females_all_rows.where('AGE', are.not_equal_to(999))` |
| `fit_table.sample` | Lấy mẫu ngẫu nhiên từ Table. | `fit_table.sample(3)` | `fit_table.sample(3)` |
| `fit_table.scatter` | Vẽ biểu đồ phân tán từ Table. | `fit_table.scatter('Fitted', 'Residuals')` | `fit_table.scatter('Fitted', 'Residuals')` |
| `fit_table.with_columns` | Thêm nhiều cột mới vào Table. | `fit_table.with_columns('1st Flr SF', train.column('1st Flr SF'),
                                  'Garage Area', train.column('Garage Area'))` | `fit_table.with_columns('1st Flr SF', train.column('1st Flr SF'),
                                  'Garage Area', train.column('Garage Area'))` |
| `fitted_income.scatter` | Vẽ biểu đồ phân tán từ Table. | `fitted_income.scatter('College%')` | `fitted_income.scatter('College%')` |
| `fitted_income.with_columns` | Thêm nhiều cột mới vào Table. | `fitted_income.with_columns('Graph of Averages',
    demographics.apply(local_average_income, 'College%'))` | `fitted_income.with_columns('Graph of Averages',
    demographics.apply(local_average_income, 'College%'))` |
| `fitted_values` | Hàm tự định nghĩa trong notebook. | `fitted_values(demographics, 'College%', 'Median Income')` | `fitted_values(demographics, 'College%', 'Median Income')` |
| `five_nearest_neighbors.where` | Lọc dòng theo điều kiện. | `five_nearest_neighbors.where('Class', are.equal_to(1))` | `five_nearest_neighbors.where('Class', are.equal_to(1))` |
| `flavor_table.barh` | Vẽ biểu đồ thanh ngang. | `flavor_table.barh('Flavor')` | `flavor_table.barh('Flavor')` |
| `float` | Chuyển giá trị sang số thực. | `float('one point two')` | `float('one point two')` |
| `full.select` | Chọn cột cần làm việc trong Table. | `full.select('AGE', 'SEX', 
            'POPESTIMATE2019', 'POPESTIMATE2011')` | `full.select('AGE', 'SEX', 
            'POPESTIMATE2019', 'POPESTIMATE2011')` |
| `group` | Nhóm dữ liệu theo giá trị cột. | `births.select('Maternal Smoker', 
              'Birth Weight').group('Maternal Smoker',np.average)` | `births.select('Maternal Smoker', 
              'Birth Weight').group('Maternal Smoker',np.average)` |
| `height_table.column` | Lấy cột dữ liệu từ Table. | `height_table.column('Percent')` | `height_table.column('Percent')` |
| `height_table.with_column` | Thêm cột mới vào Table. | `height_table.with_column('Width', bin_widths)` | `height_table.with_column('Width', bin_widths)` |
| `heights.apply` | Phương thức của đối tượng trong notebook. | `heights.apply(predict_child, 'Parent Average')` | `heights.apply(predict_child, 'Parent Average')` |
| `heights.column` | Lấy cột dữ liệu từ Table. | `heights.column('Parent Average')` | `heights.column('Parent Average')` |
| `heights.scatter` | Vẽ biểu đồ phân tán từ Table. | `heights.scatter('Parent Average', 'Child')` | `heights.scatter('Parent Average', 'Child')` |
| `heights.show` | Hiển thị nội dung Table. | `heights.show(6)` | `heights.show(6)` |
| `heights.where` | Lọc dòng theo điều kiện. | `heights.where('Parent Average', are.between(h - 1/2, h + 1/2))` | `heights.where('Parent Average', are.between(h - 1/2, h + 1/2))` |
| `heights.with_column` | Thêm cột mới vào Table. | `heights.with_column(
    'Nearest neighbor prediction', 
    heights.apply(nn_prediction_height, 'Parent Average'))` | `heights.with_column(
    'Nearest neighbor prediction', 
    heights.apply(nn_prediction_height, 'Parent Average'))` |
| `heights.with_columns` | Thêm nhiều cột mới vào Table. | `heights.with_columns(
    'Prediction', heights.apply(predict_child, 'Parent Average'))` | `heights.with_columns(
    'Prediction', heights.apply(predict_child, 'Parent Average'))` |
| `heights_with_predictions.scatter` | Vẽ biểu đồ phân tán từ Table. | `heights_with_predictions.scatter('Parent Average')` | `heights_with_predictions.scatter('Parent Average')` |
| `heights_with_predictions.show` | Hiển thị nội dung Table. | `heights_with_predictions.show(5)` | `heights_with_predictions.show(5)` |
| `heights_with_predictions.with_column` | Thêm cột mới vào Table. | `heights_with_predictions.with_column(
    'Regression Prediction', 
    predicted_heights_slope*heights.column('Parent Average') + predicted_heights_intercept
)` | `heights_with_predictions.with_column(
    'Regression Prediction', 
    predicted_heights_slope*heights.column('Parent Average') + predicted_heights_intercept
)` |
| `hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `die.sample(5).hist(bins = make_array(1,2,3,4,5,6,7),unit = 'spot')` | `die.sample(5).hist(bins = make_array(1,2,3,4,5,6,7),unit = 'spot')` |
| `huck_finn_text.split` | Phương thức của đối tượng trong notebook. | `huck_finn_text.split('CHAPTER ')` | `huck_finn_text.split('CHAPTER ')` |
| `hybrid.sample` | Lấy mẫu ngẫu nhiên từ Table. | `hybrid.sample(6)` | `hybrid.sample(6)` |
| `hybrid.scatter` | Vẽ biểu đồ phân tán từ Table. | `hybrid.scatter('acceleration', 'msrp')` | `hybrid.scatter('acceleration', 'msrp')` |
| `hybrid.where` | Lọc dòng theo điều kiện. | `hybrid.where('class', 'SUV')` | `hybrid.where('class', 'SUV')` |
| `hypotenuse` | Hàm tự định nghĩa trong notebook. | `hypotenuse(1, 2)` | `hypotenuse(1, 2)` |
| `income_residuals.show` | Hiển thị nội dung Table. | `income_residuals.show(5)` | `income_residuals.show(5)` |
| `int` | Chuyển giá trị sang số nguyên. | `int('3')` | `int('3')` |
| `intercept` | Hàm tự định nghĩa trong notebook. | `intercept(t, x, y)` | `intercept(t, x, y)` |
| `interval.item` | Lấy giá trị đơn trong hàng/array. | `interval.item(1)` | `interval.item(1)` |
| `intervals.scatter` | Vẽ biểu đồ phân tán từ Table. | `intervals.scatter('lower', 'Number', group='conf_level')` | `intervals.scatter('lower', 'Number', group='conf_level')` |
| `intervals.show` | Hiển thị nội dung Table. | `intervals.show(5)` | `intervals.show(5)` |
| `intervals.with_columns` | Thêm nhiều cột mới vào Table. | `intervals.with_columns('Number', np.arange(100) + 1)` | `intervals.with_columns('Number', np.arange(100) + 1)` |
| `intervals.with_row` | Thêm hàng vào Table. | `intervals.with_row([
            interval.item(0), interval.item(1)
        ])` | `intervals.with_row([
            interval.item(0), interval.item(1)
        ])` |
| `item` | Lấy giá trị đơn trong hàng/array. | `sample_proportions(929, predicted_proportions).item(0)` | `sample_proportions(929, predicted_proportions).item(0)` |
| `jittered.scatter` | Vẽ biểu đồ phân tán từ Table. | `jittered.scatter(0, 1, group='Class')` | `jittered.scatter(0, 1, group='Class')` |
| `join` | Nối hai Table theo khóa chung. | `test_grid.with_column('Class', c).join('Class', color_table)` | `test_grid.with_column('Class', c).join('Class', color_table)` |
| `jury.column` | Lấy cột dữ liệu từ Table. | `jury.column('Panels')` | `jury.column('Panels')` |
| `jury.with_column` | Thêm cột mới vào Table. | `jury.with_column('Difference', diffs)` | `jury.with_column('Difference', diffs)` |
| `jury_with_difference.column` | Lấy cột dữ liệu từ Table. | `jury_with_difference.column('Difference')` | `jury_with_difference.column('Difference')` |
| `jury_with_difference.where` | Lọc dòng theo điều kiện. | `jury_with_difference.where('Difference', are.above(0))` | `jury_with_difference.where('Difference', are.above(0))` |
| `jury_with_simulated.barh` | Vẽ biểu đồ thanh ngang. | `jury_with_simulated.barh('Ethnicity')` | `jury_with_simulated.barh('Ethnicity')` |
| `k_table.plot` | Vẽ biểu đồ từ Table dữ liệu. | `k_table.plot('k','MCR')` | `k_table.plot('k','MCR')` |
| `k_values.item` | Lấy giá trị đơn trong hàng/array. | `k_values.item(i)` | `k_values.item(i)` |
| `knn` | Hàm tự định nghĩa trong notebook. | `knn(train, 'Class', test, 3)` | `knn(train, 'Class', test, 3)` |
| `len` | Trả về độ dài của dãy, chuỗi hoặc tập hợp. | `len(my_array)` | `len(my_array)` |
| `line.item` | Lấy giá trị đơn trong hàng/array. | `line.item('at 291')` | `line.item('at 291')` |
| `line.scatter` | Vẽ biểu đồ phân tán từ Table. | `line.scatter('x', 'y', s=30, color='r')` | `line.scatter('x', 'y', s=30, color='r')` |
| `lines.append` | Phương thức của đối tượng trong notebook. | `lines.append([a, b, a * 210 + b, a * 300 + b, a * 320 + b])` | `lines.append([a, b, a * 210 + b, a * 300 + b, a * 320 + b])` |
| `lines.row` | Truy cập hàng trong Table hoặc tạo hàng mới. | `lines.row(i)` | `lines.row(i)` |
| `little_women_text.split` | Phương thức của đối tượng trong notebook. | `little_women_text.split('CHAPTER ')` | `little_women_text.split('CHAPTER ')` |
| `majority` | Hàm tự định nghĩa trong notebook. | `majority(five_nearest_neighbors)` | `majority(five_nearest_neighbors)` |
| `make_array` | Hàm Python hoặc method được sử dụng trong notebook. | `make_array(1,5,7,3,9)` | `make_array(1,5,7,3,9)` |
| `make_correlated_data` | Hàm tự định nghĩa trong notebook. | `make_correlated_data(r)` | `make_correlated_data(r)` |
| `males.column` | Lấy cột dữ liệu từ Table. | `males.column('2019')` | `males.column('2019')` |
| `males.show` | Hiển thị nội dung Table. | `males.show(3)` | `males.show(3)` |
| `males_all_rows.where` | Lọc dòng theo điều kiện. | `males_all_rows.where('AGE', are.not_equal_to(999))` | `males_all_rows.where('AGE', are.not_equal_to(999))` |
| `material_by_city.barh` | Vẽ biểu đồ thanh ngang. | `material_by_city.barh('city')` | `material_by_city.barh('city')` |
| `max` | Lấy giá trị lớn nhất. | `ckd.where('Class',are.equal_to(0)).column('Glucose').max()` | `ckd.where('Class',are.equal_to(0)).column('Glucose').max()` |
| `mean` | Hàm Python hoặc method được sử dụng trong notebook. | `close_points.column('Median Income').mean()` | `close_points.column('Median Income').mean()` |
| `means_array.item` | Lấy giá trị đơn trong hàng/array. | `means_array.item(1)` | `means_array.item(1)` |
| `means_table.column` | Lấy cột dữ liệu từ Table. | `means_table.column(1)` | `means_table.column(1)` |
| `means_tbl.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `means_tbl.hist(bins = np.arange(5, 31, 0.5))` | `means_tbl.hist(bins = np.arange(5, 31, 0.5))` |
| `min` | Lấy giá trị nhỏ nhất. | `min(14, 15)` | `min(14, 15)` |
| `minimize` | Hàm Python hoặc method được sử dụng trong notebook. | `minimize(f)` | `minimize(f)` |
| `monty_hall` | Hàm tự định nghĩa trong notebook. | `monty_hall()` | `monty_hall()` |
| `move_to_start` | Hàm Python hoặc method được sử dụng trong notebook. | `united.with_column('Row', np.arange(united.num_rows)).move_to_start('Row')` | `united.with_column('Row', np.arange(united.num_rows)).move_to_start('Row')` |
| `my_array.item` | Lấy giá trị đơn trong hàng/array. | `my_array.item(0)` | `my_array.item(0)` |
| `name_and_age` | Hàm tự định nghĩa trong notebook. | `name_and_age("Jeremy", 1999)` | `name_and_age("Jeremy", 1999)` |
| `nba.column` | Lấy cột dữ liệu từ Table. | `nba.column('salary')` | `nba.column('salary')` |
| `nba.drop` | Xóa cột khỏi Table. | `nba.drop('position')` | `nba.drop('position')` |
| `nba.select` | Chọn cột cần làm việc trong Table. | `nba.select('salary')` | `nba.select('salary')` |
| `nba.show` | Hiển thị nội dung Table. | `nba.show(6)` | `nba.show(6)` |
| `nba.sort` | Sắp xếp bảng theo cột. | `nba.sort('season', descending=True)` | `nba.sort('season', descending=True)` |
| `nba.where` | Lọc dòng theo điều kiện. | `nba.where('salary', are.above(15))` | `nba.where('salary', are.above(15))` |
| `nearby.column` | Lấy cột dữ liệu từ Table. | `nearby.column('Child')` | `nearby.column('Child')` |
| `nearest` | Hàm tự định nghĩa trong notebook. | `nearest(training, new_point, k)` | `nearest(training, new_point, k)` |
| `nearest_neighbors_table.group` | Nhóm dữ liệu theo giá trị cột. | `nearest_neighbors_table.group(class_name)` | `nearest_neighbors_table.group(class_name)` |
| `nearest_neighbors_table.where` | Lọc dòng theo điều kiện. | `nearest_neighbors_table.where('Class', are.equal_to(0))` | `nearest_neighbors_table.where('Class', are.equal_to(0))` |
| `neighbors.column` | Lấy cột dữ liệu từ Table. | `neighbors.column('y')` | `neighbors.column('y')` |
| `next_bs_sample.column` | Lấy cột dữ liệu từ Table. | `next_bs_sample.column(variable)` | `next_bs_sample.column(variable)` |
| `nn_5_regression_estimate` | Hàm tự định nghĩa trong notebook. | `nn_5_regression_estimate(example_row)` | `nn_5_regression_estimate(example_row)` |
| `nonlinear.scatter` | Vẽ biểu đồ phân tán từ Table. | `nonlinear.scatter('x', 'y', s=30, color='r')` | `nonlinear.scatter('x', 'y', s=30, color='r')` |
| `np.abs` | Hàm thư viện np. | `np.abs(deviations)` | `np.abs(deviations)` |
| `np.append` | Nối thêm phần tử vào mảng. | `np.append(bootstrapped_sample_medians, new_median)` | `np.append(bootstrapped_sample_medians, new_median)` |
| `np.arange` | Tạo mảng NumPy gồm các số có bước nhảy cố định. | `np.arange(num_simulations)` | `np.arange(num_simulations)` |
| `np.array` | Tạo mảng NumPy từ danh sách hoặc iterable. | `np.array(['Second'] * second + ['Third'] * third)` | `np.array(['Second'] * second + ['Third'] * third)` |
| `np.average` | Tính giá trị trung bình có trọng số. | `np.average(population.column('Total Compensation'))` | `np.average(population.column('Total Compensation'))` |
| `np.char.count` | Đếm số lần xuất hiện của chuỗi trong mảng ký tự. | `np.char.count(huck_finn_chapters, '.')` | `np.char.count(huck_finn_chapters, '.')` |
| `np.count_nonzero` | Đếm phần tử khác 0 trong mảng. | `np.count_nonzero(hundred_tosses == 'Heads')` | `np.count_nonzero(hundred_tosses == 'Heads')` |
| `np.cumsum` | Tính tổng cộng dồn của mảng. | `np.cumsum(counts.column("Meg"))` | `np.cumsum(counts.column("Meg"))` |
| `np.diff` | Tính sai khác giữa các phần tử liên tiếp. | `np.diff(binned_data.column('bin'))` | `np.diff(binned_data.column('bin'))` |
| `np.max` | Tìm giá trị lớn nhất. | `np.max(population.column('Total Compensation'))` | `np.max(population.column('Total Compensation'))` |
| `np.mean` | Tính trung bình cộng của mảng. | `np.mean(heights)` | `np.mean(heights)` |
| `np.median` | Tính trung vị của mảng. | `np.median(united.column('Delay'))` | `np.median(united.column('Delay'))` |
| `np.min` | Tìm giá trị nhỏ nhất. | `np.min(x)` | `np.min(x)` |
| `np.ones` | Tạo mảng NumPy toàn số 1. | `np.ones(number_of_ones)` | `np.ones(number_of_ones)` |
| `np.random.choice` | Lấy mẫu ngẫu nhiên từ một tập hợp. | `np.random.choice(coin, 100)` | `np.random.choice(coin, 100)` |
| `np.random.normal` | Tạo mẫu từ phân phối chuẩn. | `np.random.normal(50, 5, sample_size)` | `np.random.normal(50, 5, sample_size)` |
| `np.random.seed` | Khóa hạt giống cho tạo số ngẫu nhiên. | `np.random.seed(8)` | `np.random.seed(8)` |
| `np.round` | Làm tròn giá trị. | `np.round(top10_adjusted.column('Gross (Adjusted)') / 1000000, 3)` | `np.round(top10_adjusted.column('Gross (Adjusted)') / 1000000, 3)` |
| `np.sin` | Tính sin của giá trị. | `np.sin(x*np.pi)` | `np.sin(x*np.pi)` |
| `np.size` | Trả về kích thước của mảng. | `np.size(k_values)` | `np.size(k_values)` |
| `np.sqrt` | Tính căn bậc hai. | `np.sqrt(sample_sizes)` | `np.sqrt(sample_sizes)` |
| `np.std` | Tính độ lệch chuẩn của mảng. | `np.std(ages)` | `np.std(ages)` |
| `np.sum` | Tính tổng các phần tử mảng. | `np.sum(values)` | `np.sum(values)` |
| `np.zeros` | Tạo mảng NumPy toàn số 0. | `np.zeros(10 - number_of_ones)` | `np.zeros(10 - number_of_ones)` |
| `observed_die_distribution` | Hàm tự định nghĩa trong notebook. | `observed_die_distribution(10)` | `observed_die_distribution(10)` |
| `observed_die_rolls.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `observed_die_rolls.hist(bins = make_array(1,2,3,4,5,6,7),unit = 'spot')` | `observed_die_rolls.hist(bins = make_array(1,2,3,4,5,6,7),unit = 'spot')` |
| `observed_sample_median` | Hàm tự định nghĩa trong notebook. | `observed_sample_median(sample_size)` | `observed_sample_median(sample_size)` |
| `observed_sample_median_distribution` | Hàm tự định nghĩa trong notebook. | `observed_sample_median_distribution(1000,100)` | `observed_sample_median_distribution(1000,100)` |
| `one_bootstrap_median` | Hàm tự định nghĩa trong notebook. | `one_bootstrap_median()` | `one_bootstrap_median()` |
| `one_knn` | Hàm tự định nghĩa trong notebook. | `one_knn(training, 
                                                     class_name, 
                                                     testing.drop(class_name).row(i), 
                                                     k)` | `one_knn(training, 
                                                     class_name, 
                                                     testing.drop(class_name).row(i), 
                                                     k)` |
| `one_million_roll_table.take` | Lấy các hàng chỉ định theo chỉ số. | `one_million_roll_table.take(np.arange(start, start + 1000))` | `one_million_roll_table.take(np.arange(start, start + 1000))` |
| `one_sample_average` | Hàm tự định nghĩa trong notebook. | `one_sample_average()` | `one_sample_average()` |
| `one_sample_mean` | Hàm tự định nghĩa trong notebook. | `one_sample_mean(sample_size)` | `one_sample_mean(sample_size)` |
| `one_simulated_value` | Hàm tự định nghĩa trong notebook. | `one_simulated_value()` | `one_simulated_value()` |
| `one_step` | Hàm tự định nghĩa trong notebook. | `one_step()` | `one_step()` |
| `original_sample.sample` | Lấy mẫu ngẫu nhiên từ Table. | `original_sample.sample(k = original_sample.num_rows, with_replacement = True)` | `original_sample.sample(k = original_sample.num_rows, with_replacement = True)` |
| `other_goat` | Hàm tự định nghĩa trong notebook. | `other_goat(monty_choice)` | `other_goat(monty_choice)` |
| `outlier.scatter` | Vẽ biểu đồ phân tán từ Table. | `outlier.scatter('x', 'y', s=30, color='r')` | `outlier.scatter('x', 'y', s=30, color='r')` |
| `panel_proportion` | Hàm tự định nghĩa trong notebook. | `panel_proportion()` | `panel_proportion()` |
| `partial.relabeled` | Phương thức của đối tượng trong notebook. | `partial.relabeled(2, '2019')` | `partial.relabeled(2, '2019')` |
| `partial.show` | Hiển thị nội dung Table. | `partial.show(5)` | `partial.show(5)` |
| `patient.item` | Lấy giá trị đơn trong hàng/array. | `patient.item(1)` | `patient.item(1)` |
| `patients.column` | Lấy cột dữ liệu từ Table. | `patients.column('Bland Chromatin')` | `patients.column('Bland Chromatin')` |
| `patients.group` | Nhóm dữ liệu theo giá trị cột. | `patients.group('Class')` | `patients.group('Class')` |
| `patients.sample` | Lấy mẫu ngẫu nhiên từ Table. | `patients.sample(5)` | `patients.sample(5)` |
| `patients.scatter` | Vẽ biểu đồ phân tán từ Table. | `patients.scatter('Bland Chromatin', 'Single Epithelial Cell Size', group='Class')` | `patients.scatter('Bland Chromatin', 'Single Epithelial Cell Size', group='Class')` |
| `patients.select` | Chọn cột cần làm việc trong Table. | `patients.select('Single Epithelial Cell Size','Bland Chromatin', 'Class')` | `patients.select('Single Epithelial Cell Size','Bland Chromatin', 'Class')` |
| `patients.split` | Phương thức của đối tượng trong notebook. | `patients.split(k = round(patients.num_rows/2))` | `patients.split(k = round(patients.num_rows/2))` |
| `percentile` | Hàm Python hoặc method được sử dụng trong notebook. | `percentile((100-confidence_level)/2, bootstrap_stats)` | `percentile((100-confidence_level)/2, bootstrap_stats)` |
| `pivot` | Biến đổi bảng theo hàng/cột. | `skyscrapers.select('city', 'material', 
                   'height').pivot('material','city',values = 'height', collect = max)` | `skyscrapers.select('city', 'material', 
                   'height').pivot('material','city',values = 'height', collect = max)` |
| `plot` | Vẽ biểu đồ từ Table dữ liệu. | `Table().with_columns('x', x, 'y', y).plot('x')` | `Table().with_columns('x', x, 'y', y).plot('x')` |
| `plot_all_points` | Hàm tự định nghĩa trong notebook. | `plot_all_points(test_grid)` | `plot_all_points(test_grid)` |
| `plot_all_points_classified` | Hàm tự định nghĩa trong notebook. | `plot_all_points_classified(test_grid)` | `plot_all_points_classified(test_grid)` |
| `plot_fitted` | Hàm tự định nghĩa trong notebook. | `plot_fitted(heights, 'Parent Average', 'Child')` | `plot_fitted(heights, 'Parent Average', 'Child')` |
| `plot_residuals` | Hàm tự định nghĩa trong notebook. | `plot_residuals(us_women, 'height', 'ave weight')` | `plot_residuals(us_women, 'height', 'ave weight')` |
| `plot_sample_mean_distribution` | Hàm tự định nghĩa trong notebook. | `plot_sample_mean_distribution(100)` | `plot_sample_mean_distribution(100)` |
| `plot_sample_means` | Hàm tự định nghĩa trong notebook. | `plot_sample_means(625)` | `plot_sample_means(625)` |
| `plots.figure` | Tạo khung đồ họa cho plots. | `plots.figure(figsize=(5,5))` | `plots.figure(figsize=(5,5))` |
| `plots.plot` | Vẽ biểu đồ tuyến. | `plots.plot([210, 320], [line.item('at 210'), line.item('at 320')], lw=1)` | `plots.plot([210, 320], [line.item('at 210'), line.item('at 320')], lw=1)` |
| `plots.scatter` | Vẽ biểu đồ phân tán. | `plots.scatter(68, nearby_mean, color='red', s=50)` | `plots.scatter(68, nearby_mean, color='red', s=50)` |
| `plots.style.use` | Chọn kiểu đồ họa. | `plots.style.use('fivethirtyeight')` | `plots.style.use('fivethirtyeight')` |
| `plots.subplot` | Tạo nhiều đồ thị con trong một khung. | `plots.subplot(3,2,i+1)` | `plots.subplot(3,2,i+1)` |
| `plots.suptitle` | Thiết lập tiêu đề chung cho nhiều biểu đồ. | `plots.suptitle('\n \n 95 percent confidence intervals', y = 1)` | `plots.suptitle('\n \n 95 percent confidence intervals', y = 1)` |
| `plots.tight_layout` | Tự động căn chỉnh layout đồ họa. | `plots.tight_layout()` | `plots.tight_layout()` |
| `plots.title` | Thiết lập tiêu đề biểu đồ. | `plots.title('Average as a Center of Mass')` | `plots.title('Average as a Center of Mass')` |
| `plots.xlabel` | Thiết lập nhãn trục x. | `plots.xlabel('Sample Means')` | `plots.xlabel('Sample Means')` |
| `plots.xlim` | Thiết lập giới hạn trục x. | `plots.xlim([225, 325])` | `plots.xlim([225, 325])` |
| `plots.xticks` | Thiết lập vị trí và nhãn trục x. | `plots.xticks(np.arange(57, 72, 2))` | `plots.xticks(np.arange(57, 72, 2))` |
| `plots.ylim` | Thiết lập giới hạn trục y. | `plots.ylim(-0.02*100, 0.6*100)` | `plots.ylim(-0.02*100, 0.6*100)` |
| `plt.figure` | Tạo một khung hình mới để vẽ đồ thị. | `plt.figure(figsize=(8,8))` | `plt.figure(figsize=(8,8))` |
| `plt.plot` | Vẽ đường thẳng hoặc đồ thị tuyến tính. | `plt.plot([210, 320], [line.item('at 210'), line.item('at 320')], lw=1)` | `plt.plot([210, 320], [line.item('at 210'), line.item('at 320')], lw=1)` |
| `plt.scatter` | Vẽ biểu đồ phân tán. | `plt.scatter(point.item(0), point.item(1), color='red', s=30)` | `plt.scatter(point.item(0), point.item(1), color='red', s=30)` |
| `plt.show` | Hiển thị đồ thị. | `plt.show()` | `plt.show()` |
| `plt.title` | Thiết lập tiêu đề biểu đồ. | `plt.title('Cumulative Number of Times Names Appear in Little Women')` | `plt.title('Cumulative Number of Times Names Appear in Little Women')` |
| `plt.xlabel` | Thiết lập nhãn trục x. | `plt.xlabel('Number of periods in chapter')` | `plt.xlabel('Number of periods in chapter')` |
| `plt.xlim` | Thiết lập giới hạn trục x. | `plt.xlim(-2, 2)` | `plt.xlim(-2, 2)` |
| `plt.ylabel` | Thiết lập nhãn trục y. | `plt.ylabel('Number of characters in chapter')` | `plt.ylabel('Number of characters in chapter')` |
| `plt.ylim` | Thiết lập giới hạn trục y. | `plt.ylim(-2, 2)` | `plt.ylim(-2, 2)` |
| `point.item` | Lấy giá trị đơn trong hàng/array. | `point.item(0)` | `point.item(0)` |
| `point_guards.drop` | Xóa cột khỏi Table. | `point_guards.drop('rank', 'position', 'season')` | `point_guards.drop('rank', 'position', 'season')` |
| `point_guards.show` | Hiển thị nội dung Table. | `point_guards.show(10)` | `point_guards.show(10)` |
| `point_guards.sort` | Sắp xếp bảng theo cột. | `point_guards.sort('salary', descending=True)` | `point_guards.sort('salary', descending=True)` |
| `population.column` | Lấy cột dữ liệu từ Table. | `population.column('Total Compensation')` | `population.column('Total Compensation')` |
| `population.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `population.hist('Total Compensation', bins = np.arange(0, 800000, 25000))` | `population.hist('Total Compensation', bins = np.arange(0, 800000, 25000))` |
| `population.sample` | Lấy mẫu ngẫu nhiên từ Table. | `population.sample(30, with_replacement=False)` | `population.sample(30, with_replacement=False)` |
| `population.sort` | Sắp xếp bảng theo cột. | `population.sort('Total Compensation', descending=True)` | `population.sort('Total Compensation', descending=True)` |
| `population.where` | Lọc dòng theo điều kiện. | `population.where('Salary', are.above(min_salary))` | `population.where('Salary', are.above(min_salary))` |
| `predicted.item` | Lấy giá trị đơn trong hàng/array. | `predicted.item(0)` | `predicted.item(0)` |
| `prediction_at` | Hàm tự định nghĩa trong notebook. | `prediction_at(resample, x, y, new_x)` | `prediction_at(resample, x, y, new_x)` |
| `print` | In ra nội dung ra màn hình. | `print(round_left, 'to', round_right, '( width =', round(right - left, 3), ')')` | `print(round_left, 'to', round_right, '( width =', round(right - left, 3), ')')` |
| `proportions` | Hàm tự định nghĩa trong notebook. | `proportions(remaining_grouped.column('count'))` | `proportions(remaining_grouped.column('count'))` |
| `purple_flowers` | Hàm tự định nghĩa trong notebook. | `purple_flowers()` | `purple_flowers()` |
| `quantity_function` | Hàm Python hoặc method được sử dụng trong notebook. | `quantity_function(next_bs_sample.column(variable))` | `quantity_function(next_bs_sample.column(variable))` |
| `r_scatter` | Hàm tự định nghĩa trong notebook. | `r_scatter(1)` | `r_scatter(1)` |
| `r_table` | Hàm tự định nghĩa trong notebook. | `r_table(0)` | `r_table(0)` |
| `random_section.column` | Lấy cột dữ liệu từ Table. | `random_section.column('Midterm')` | `random_section.column('Midterm')` |
| `randomize_column` | Hàm tự định nghĩa trong notebook. | `randomize_column(patients.column('Single Epithelial Cell Size'))` | `randomize_column(patients.column('Single Epithelial Cell Size'))` |
| `range` | Tạo dãy số nguyên. | `range(test.num_rows)` | `range(test.num_rows)` |
| `ratios.plot` | Vẽ biểu đồ từ Table dữ liệu. | `ratios.plot('Age', 'F:M Ratio')` | `ratios.plot('Age', 'F:M Ratio')` |
| `ratios.show` | Hiển thị nội dung Table. | `ratios.show(6)` | `ratios.show(6)` |
| `ratios.sort` | Sắp xếp bảng theo cột. | `ratios.sort('Age', descending=True)` | `ratios.sort('Age', descending=True)` |
| `re.sub` | Thay thế phần chuỗi khớp regex. | `re.sub('\\s+', ' ', urlopen(url).read().decode())` | `re.sub('\\s+', ' ', urlopen(url).read().decode())` |
| `read` | Hàm Python hoặc method được sử dụng trong notebook. | `urlopen(url).read()` | `urlopen(url).read()` |
| `read_table` | Đọc dữ liệu vào Table từ CSV. | `Table().read_table('breast-cancer.csv')` | `Table().read_table('breast-cancer.csv')` |
| `read_url` | Hàm tự định nghĩa trong notebook. | `read_url(huck_finn_url)` | `read_url(huck_finn_url)` |
| `recent_curry.column` | Lấy cột dữ liệu từ Table. | `recent_curry.column('salary')` | `recent_curry.column('salary')` |
| `recent_curry.select` | Chọn cột cần làm việc trong Table. | `recent_curry.select('salary')` | `recent_curry.select('salary')` |
| `relabeled` | Hàm Python hoặc method được sử dụng trong notebook. | `partial.relabeled(2, '2014').relabeled(3, '2019')` | `partial.relabeled(2, '2014').relabeled(3, '2019')` |
| `remaining_grouped.barh` | Vẽ biểu đồ thanh ngang. | `remaining_grouped.barh('Remaining')` | `remaining_grouped.barh('Remaining')` |
| `remaining_grouped.column` | Lấy cột dữ liệu từ Table. | `remaining_grouped.column('count')` | `remaining_grouped.column('count')` |
| `resample.column` | Lấy cột dữ liệu từ Table. | `resample.column('Total Compensation')` | `resample.column('Total Compensation')` |
| `resample.scatter` | Vẽ biểu đồ phân tán từ Table. | `resample.scatter('Gestational Days', 'Birth Weight', fit_line=True)` | `resample.scatter('Gestational Days', 'Birth Weight', fit_line=True)` |
| `resampled.column` | Lấy cột dữ liệu từ Table. | `resampled.column('Gestational Days')` | `resampled.column('Gestational Days')` |
| `resampled_means.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `resampled_means.hist(bins=15)` | `resampled_means.hist(bins=15)` |
| `residuals` | Hàm tự định nghĩa trong notebook. | `residuals(heights, 'Parent Average', 'Child')` | `residuals(heights, 'Parent Average', 'Child')` |
| `resize_window` | Hàm tự định nghĩa trong notebook. | `resize_window()` | `resize_window()` |
| `results.append` | Phương thức của đối tượng trong notebook. | `results.append(three_card_game())` | `results.append(three_card_game())` |
| `results.column` | Lấy cột dữ liệu từ Table. | `results.column('Predicted')` | `results.column('Predicted')` |
| `results.group` | Nhóm dữ liệu theo giá trị cột. | `results.group("Contestant's Choice")` | `results.group("Contestant's Choice")` |
| `results.show` | Hiển thị nội dung Table. | `results.show(3)` | `results.show(3)` |
| `results_grouped.column` | Lấy cột dữ liệu từ Table. | `results_grouped.column('count')` | `results_grouped.column('count')` |
| `results_grouped.with_column` | Thêm cột mới vào Table. | `results_grouped.with_column('Proportion',(card_counts/total_simulations))` | `results_grouped.with_column('Proportion',(card_counts/total_simulations))` |
| `rg.apply` | Phương thức của đối tượng trong notebook. | `rg.apply(percent_growth, '2023', '2024')` | `rg.apply(percent_growth, '2023', '2024')` |
| `rg.column` | Lấy cột dữ liệu từ Table. | `rg.column('2023')` | `rg.column('2023')` |
| `rg.sort` | Sắp xếp bảng theo cột. | `rg.sort('Transactions YOY', descending=True)` | `rg.sort('Transactions YOY', descending=True)` |
| `rg.with_columns` | Thêm nhiều cột mới vào Table. | `rg.with_columns('Transactions YOY', rg.apply(percent_growth, '2023', '2024'))` | `rg.with_columns('Transactions YOY', rg.apply(percent_growth, '2023', '2024'))` |
| `round` | Làm tròn số. | `round(no_disease * 0.05)` | `round(no_disease * 0.05)` |
| `row` | Truy cập hàng trong Table hoặc tạo hàng mới. | `banknotes.drop('Class').row(0)` | `banknotes.drop('Class').row(0)` |
| `row.item` | Lấy giá trị đơn trong hàng/array. | `row.item('Number')` | `row.item('Number')` |
| `sales.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `sales.hist('SalePrice', bins=32, unit='$')` | `sales.hist('SalePrice', bins=32, unit='$')` |
| `sales.sample` | Lấy mẫu ngẫu nhiên từ Table. | `sales.sample(with_replacement = False)` | `sales.sample(with_replacement = False)` |
| `sales.scatter` | Vẽ biểu đồ phân tán từ Table. | `sales.scatter('1st Flr SF', 'SalePrice')` | `sales.scatter('1st Flr SF', 'SalePrice')` |
| `sales.select` | Chọn cột cần làm việc trong Table. | `sales.select(0, 1, 2, 3, 4, 8)` | `sales.select(0, 1, 2, 3, 4, 8)` |
| `sales.show` | Hiển thị nội dung Table. | `sales.show(3)` | `sales.show(3)` |
| `sales_estimate` | Hàm tự định nghĩa trong notebook. | `sales_estimate(train, 7.99370803e+01,   7.72401282e+01,   5.23616519e+01,
         4.68487623e+01,   5.61174620e+02,  -1.11909133e+06)` | `sales_estimate(train, 7.99370803e+01,   7.72401282e+01,   5.23616519e+01,
         4.68487623e+01,   5.61174620e+02,  -1.11909133e+06)` |
| `sales_shuffled.take` | Lấy các hàng chỉ định theo chỉ số. | `sales_shuffled.take(np.arange(halfway_split_point))` | `sales_shuffled.take(np.arange(halfway_split_point))` |
| `sales_test_rmse` | Hàm tự định nghĩa trong notebook. | `sales_test_rmse(8.57001834e+01,   8.31651700e+01,   4.78808900e+01,
         5.18150471e+01,   5.19933651e+02,  -1.04414307e+06)` | `sales_test_rmse(8.57001834e+01,   8.31651700e+01,   4.78808900e+01,
         5.18150471e+01,   5.19933651e+02,  -1.04414307e+06)` |
| `sample` | Lấy mẫu ngẫu nhiên từ Table. | `births.select('Maternal Smoker').sample(with_replacement=False)` | `births.select('Maternal Smoker').sample(with_replacement=False)` |
| `sample.scatter` | Vẽ biểu đồ phân tán từ Table. | `sample.scatter('x', 'y', fit_line=True)` | `sample.scatter('x', 'y', fit_line=True)` |
| `sample_10.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `sample_10.hist('Delay', bins = delay_bins, unit = 'minute')` | `sample_10.hist('Delay', bins = delay_bins, unit = 'minute')` |
| `sample_means_tbl.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `sample_means_tbl.hist(bins=20)` | `sample_means_tbl.hist(bins=20)` |
| `sample_median_table.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `sample_median_table.hist()` | `sample_median_table.hist()` |
| `sample_proportions` | Hàm Python hoặc method được sử dụng trong notebook. | `sample_proportions(10, population_proportions)` | `sample_proportions(10, population_proportions)` |
| `sampled_flights.column` | Lấy cột dữ liệu từ Table. | `sampled_flights.column('Delay')` | `sampled_flights.column('Delay')` |
| `sat2014.apply` | Phương thức của đối tượng trong notebook. | `sat2014.apply(rate_code, 'Participation Rate')` | `sat2014.apply(rate_code, 'Participation Rate')` |
| `sat2014.scatter` | Vẽ biểu đồ phân tán từ Table. | `sat2014.scatter('Critical Reading', 'Math', group='Rate Code')` | `sat2014.scatter('Critical Reading', 'Math', group='Rate Code')` |
| `sat2014.with_columns` | Thêm nhiều cột mới vào Table. | `sat2014.with_columns('Rate Code', rate_codes)` | `sat2014.with_columns('Rate Code', rate_codes)` |
| `scatter` | Vẽ biểu đồ phân tán từ Table. | `tbl.select(x, y, 'Fitted').scatter(0)` | `tbl.select(x, y, 'Fitted').scatter(0)` |
| `scores.group` | Nhóm dữ liệu theo giá trị cột. | `scores.group('Section')` | `scores.group('Section')` |
| `scores.sample` | Lấy mẫu ngẫu nhiên từ Table. | `scores.sample(27, with_replacement=False)` | `scores.sample(27, with_replacement=False)` |
| `scores.show` | Hiển thị nội dung Table. | `scores.show(5)` | `scores.show(5)` |
| `sd_table.scatter` | Vẽ biểu đồ phân tán từ Table. | `sd_table.scatter('Sample size')` | `sd_table.scatter('Sample size')` |
| `sd_table.with_column` | Thêm cột mới vào Table. | `sd_table.with_column('Squared Deviation', deviations ** 2)` | `sd_table.with_column('Squared Deviation', deviations ** 2)` |
| `select` | Chọn cột cần làm việc trong Table. | `all_sales.where('Bldg Type', '1Fam').where('Sale Condition', 'Normal').select(
    'SalePrice', '1st Flr SF', '2nd Flr SF', 
    'Total Bsmt SF', 'Garage Area', 
    'Wood Deck SF', 'Open Porch SF', 'Lot Area', 
    'Year Built', 'Yr Sold')` | `all_sales.where('Bldg Type', '1Fam').where('Sale Condition', 'Normal').select(
    'SalePrice', '1st Flr SF', '2nd Flr SF', 
    'Total Bsmt SF', 'Garage Area', 
    'Wood Deck SF', 'Open Porch SF', 'Lot Area', 
    'Year Built', 'Yr Sold')` |
| `sf_ny_chi.pivot` | Biến đổi bảng theo hàng/cột. | `sf_ny_chi.pivot('material', 'city')` | `sf_ny_chi.pivot('material', 'city')` |
| `shotput.column` | Lấy cột dữ liệu từ Table. | `shotput.column('Weight Lifted')` | `shotput.column('Weight Lifted')` |
| `shotput.scatter` | Vẽ biểu đồ phân tán từ Table. | `shotput.scatter('Weight Lifted')` | `shotput.scatter('Weight Lifted')` |
| `shotput.show` | Hiển thị nội dung Table. | `shotput.show(6)` | `shotput.show(6)` |
| `shotput.with_column` | Thêm cột mới vào Table. | `shotput.with_column(
    'Best Line', linear_fit
)` | `shotput.with_column(
    'Best Line', linear_fit
)` |
| `shotput_linear_rmse` | Hàm tự định nghĩa trong notebook. | `shotput_linear_rmse(0.09834382,  5.95962883)` | `shotput_linear_rmse(0.09834382,  5.95962883)` |
| `shotput_quadratic_rmse` | Hàm tự định nghĩa trong notebook. | `shotput_quadratic_rmse(-1.04003731e-03,   2.82706003e-01,  -1.53167618e+00)` | `shotput_quadratic_rmse(-1.04003731e-03,   2.82706003e-01,  -1.53167618e+00)` |
| `show` | Hiển thị nội dung Table. | `ratios.sort('Age', descending=True).show(5)` | `ratios.sort('Age', descending=True).show(5)` |
| `show_closest` | Hàm tự định nghĩa trong notebook. | `show_closest(alice)` | `show_closest(alice)` |
| `show_demographics_rmse` | Hàm tự định nghĩa trong notebook. | `show_demographics_rmse(regression_slope, regression_intercept)` | `show_demographics_rmse(regression_slope, regression_intercept)` |
| `shuffled.take` | Lấy các hàng chỉ định theo chỉ số. | `shuffled.take(np.arange(halfway, patients.num_rows))` | `shuffled.take(np.arange(halfway, patients.num_rows))` |
| `shuffled_banknotes.take` | Lấy các hàng chỉ định theo chỉ số. | `shuffled_banknotes.take(np.arange(halfway))` | `shuffled_banknotes.take(np.arange(halfway))` |
| `shuffled_ckd.take` | Lấy các hàng chỉ định theo chỉ số. | `shuffled_ckd.take(np.arange(79, 158))` | `shuffled_ckd.take(np.arange(79, 158))` |
| `shuffled_group.column` | Lấy cột dữ liệu từ Table. | `shuffled_group.column(0)` | `shuffled_group.column(0)` |
| `shuffled_group.show` | Hiển thị nội dung Table. | `shuffled_group.show(5)` | `shuffled_group.show(5)` |
| `shuffled_patients.take` | Lấy các hàng chỉ định theo chỉ số. | `shuffled_patients.take(np.arange(halfway, patients.num_rows))` | `shuffled_patients.take(np.arange(halfway, patients.num_rows))` |
| `shuffled_train.take` | Lấy các hàng chỉ định theo chỉ số. | `shuffled_train.take(np.arange(seventy))` | `shuffled_train.take(np.arange(seventy))` |
| `sign` | Hàm tự định nghĩa trong notebook. | `sign(0)` | `sign(0)` |
| `simulated_abs_difference` | Hàm tự định nghĩa trong notebook. | `simulated_abs_difference(back_pain, 'Group', 'Result', np.average)` | `simulated_abs_difference(back_pain, 'Group', 'Result', np.average)` |
| `simulated_births.group` | Nhóm dữ liệu theo giá trị cột. | `simulated_births.group('Shuffled Maternal Smoker',np.average)` | `simulated_births.group('Shuffled Maternal Smoker',np.average)` |
| `simulated_births.show` | Hiển thị nội dung Table. | `simulated_births.show(5)` | `simulated_births.show(5)` |
| `simulated_difference` | Hàm tự định nghĩa trong notebook. | `simulated_difference(births, 'Maternal Smoker', 'Birth Weight', np.average)` | `simulated_difference(births, 'Maternal Smoker', 'Birth Weight', np.average)` |
| `simulated_table.group` | Nhóm dữ liệu theo giá trị cột. | `simulated_table.group(group_label, function)` | `simulated_table.group(group_label, function)` |
| `simulated_tvd` | Hàm tự định nghĩa trong notebook. | `simulated_tvd()` | `simulated_tvd()` |
| `simulation_results.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `simulation_results.hist('Number of Heads', bins = np.arange(30.5, 69.6, 1))` | `simulation_results.hist('Number of Heads', bins = np.arange(30.5, 69.6, 1))` |
| `skyscrapers.pivot` | Biến đổi bảng theo hàng/cột. | `skyscrapers.pivot('material', 'city', 
                                        values='height', collect=max)` | `skyscrapers.pivot('material', 'city', 
                                        values='height', collect=max)` |
| `skyscrapers.select` | Chọn cột cần làm việc trong Table. | `skyscrapers.select('city', 'material', 
                   'height')` | `skyscrapers.select('city', 'material', 
                   'height')` |
| `skyscrapers.show` | Hiển thị nội dung Table. | `skyscrapers.show(6)` | `skyscrapers.show(6)` |
| `skyscrapers.where` | Lọc dòng theo điều kiện. | `skyscrapers.where('city', are.contained_in(cities_we_want))` | `skyscrapers.where('city', are.contained_in(cities_we_want))` |
| `skyscrapers_pivoted.column` | Lấy cột dữ liệu từ Table. | `skyscrapers_pivoted.column('concrete')` | `skyscrapers_pivoted.column('concrete')` |
| `skyscrapers_pivoted.sort` | Sắp xếp bảng theo cột. | `skyscrapers_pivoted.sort('difference', descending=True)` | `skyscrapers_pivoted.sort('difference', descending=True)` |
| `skyscrapers_pivoted.with_column` | Thêm cột mới vào Table. | `skyscrapers_pivoted.with_column(
    'difference', 
    abs(skyscrapers_pivoted.column('steel') - 
        skyscrapers_pivoted.column('concrete'))
)` | `skyscrapers_pivoted.with_column(
    'difference', 
    abs(skyscrapers_pivoted.column('steel') - 
        skyscrapers_pivoted.column('concrete'))
)` |
| `slope` | Hàm tự định nghĩa trong notebook. | `slope(births, 'Gestational Days', 'Birth Weight')` | `slope(births, 'Gestational Days', 'Birth Weight')` |
| `sort` | Sắp xếp bảng theo cột. | `top_movies.group('Studio').sort('count', descending=True)` | `top_movies.group('Studio').sort('count', descending=True)` |
| `sorted_averages.item` | Lấy giá trị đơn trong hàng/array. | `sorted_averages.item(five_percent_index)` | `sorted_averages.item(five_percent_index)` |
| `sorted_by_distance.take` | Lấy các hàng chỉ định theo chỉ số. | `sorted_by_distance.take(np.arange(k))` | `sorted_by_distance.take(np.arange(k))` |
| `southside.with_column` | Thêm cột mới vào Table. | `southside.with_column('Blocks from campus', 
                      np.arange(4))` | `southside.with_column('Blocks from campus', 
                      np.arange(4))` |
| `sqrt` | Hàm Python hoặc method được sử dụng trong notebook. | `sqrt(x**2 + y**2)` | `sqrt(x**2 + y**2)` |
| `standard_units` | Hàm tự định nghĩa trong notebook. | `standard_units(test.column('Single Epithelial Cell Size'))` | `standard_units(test.column('Single Epithelial Cell Size'))` |
| `stats_array.item` | Lấy giá trị đơn trong hàng/array. | `stats_array.item(0)` | `stats_array.item(0)` |
| `std_ckd_results.column` | Lấy cột dữ liệu từ Table. | `std_ckd_results.column('Predicted')` | `std_ckd_results.column('Predicted')` |
| `str` | Chuyển giá trị sang chuỗi. | `str(10)` | `str(10)` |
| `students.pivot` | Biến đổi bảng theo hàng/cột. | `students.pivot('Major', 'Year')` | `students.pivot('Major', 'Year')` |
| `students.show` | Hiển thị nội dung Table. | `students.show(3)` | `students.show(3)` |
| `students.with_rows` | Phương thức của đối tượng trong notebook. | `students.with_rows(make_array(make_array('Third', 'Declared')))` | `students.with_rows(make_array(make_array('Third', 'Declared')))` |
| `studio_distribution.barh` | Vẽ biểu đồ thanh ngang. | `studio_distribution.barh('Studio')` | `studio_distribution.barh('Studio')` |
| `studio_distribution.show` | Hiển thị nội dung Table. | `studio_distribution.show(6)` | `studio_distribution.show(6)` |
| `studio_distribution.sort` | Sắp xếp bảng theo cột. | `studio_distribution.sort('count', descending=True)` | `studio_distribution.sort('count', descending=True)` |
| `sum` | Tính tổng các phần tử. | `sum(jury_with_difference.column('Difference'))` | `sum(jury_with_difference.column('Difference'))` |
| `suv.scatter` | Vẽ biểu đồ phân tán từ Table. | `suv.scatter('acceleration', 'msrp')` | `suv.scatter('acceleration', 'msrp')` |
| `t.column` | Lấy cột dữ liệu từ Table. | `t.column('product of standard units')` | `t.column('product of standard units')` |
| `t.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `t.hist(bins=20)` | `t.hist(bins=20)` |
| `t.pivot` | Biến đổi bảng theo hàng/cột. | `t.pivot('Test Result', 'Status')` | `t.pivot('Test Result', 'Status')` |
| `t.row` | Truy cập hàng trong Table hoặc tạo hàng mới. | `t.row(0)` | `t.row(0)` |
| `t.sample` | Lấy mẫu ngẫu nhiên từ Table. | `t.sample()` | `t.sample()` |
| `t.scatter` | Vẽ biểu đồ phân tán từ Table. | `t.scatter('x', 'y', s=30, color='red')` | `t.scatter('x', 'y', s=30, color='red')` |
| `t.with_columns` | Thêm nhiều cột mới vào Table. | `t.with_columns(
    'product of standard units', t.column(3) * t.column(2))` | `t.with_columns(
    'product of standard units', t.column(3) * t.column(2))` |
| `table.column` | Lấy cột dữ liệu từ Table. | `table.column(numeric_label)` | `table.column(numeric_label)` |
| `table.select` | Chọn cột cần làm việc trong Table. | `table.select(group_label)` | `table.select(group_label)` |
| `table_with_distances` | Hàm tự định nghĩa trong notebook. | `table_with_distances(training, new_point)` | `table_with_distances(training, new_point)` |
| `take` | Lấy các hàng chỉ định theo chỉ số. | `ckd.drop('Class').take(np.arange(5))` | `ckd.drop('Class').take(np.arange(5))` |
| `tbl.scatter` | Vẽ biểu đồ phân tán từ Table. | `tbl.scatter(x, 'Residual')` | `tbl.scatter(x, 'Residual')` |
| `tbl.select` | Chọn cột cần làm việc trong Table. | `tbl.select(x, y, 'Fitted')` | `tbl.select(x, y, 'Fitted')` |
| `ten_thousand_sample_means` | Hàm tự định nghĩa trong notebook. | `ten_thousand_sample_means(400)` | `ten_thousand_sample_means(400)` |
| `test.column` | Lấy cột dữ liệu từ Table. | `test.column('Total Bsmt SF')` | `test.column('Total Bsmt SF')` |
| `test.drop` | Xóa cột khỏi Table. | `test.drop(0)` | `test.drop(0)` |
| `test.row` | Truy cập hàng trong Table hoặc tạo hàng mới. | `test.row(i)` | `test.row(i)` |
| `test.select` | Chọn cột cần làm việc trong Table. | `test.select('Class')` | `test.select('Class')` |
| `test_grid.scatter` | Vẽ biểu đồ phân tán từ Table. | `test_grid.scatter('Hemoglobin', 'Glucose', color='red', alpha=0.4, s=30)` | `test_grid.scatter('Hemoglobin', 'Glucose', color='red', alpha=0.4, s=30)` |
| `test_grid.with_column` | Thêm cột mới vào Table. | `test_grid.with_column('Class', c)` | `test_grid.with_column('Class', c)` |
| `testing.column` | Lấy cột dữ liệu từ Table. | `testing.column(class_name)` | `testing.column(class_name)` |
| `testing.drop` | Xóa cột khỏi Table. | `testing.drop(class_name)` | `testing.drop(class_name)` |
| `three_card_game` | Hàm tự định nghĩa trong notebook. | `three_card_game()` | `three_card_game()` |
| `top10_adjusted.barh` | Vẽ biểu đồ thanh ngang. | `top10_adjusted.barh('Title', 'Millions')` | `top10_adjusted.barh('Title', 'Millions')` |
| `top10_adjusted.column` | Lấy cột dữ liệu từ Table. | `top10_adjusted.column('Gross (Adjusted)')` | `top10_adjusted.column('Gross (Adjusted)')` |
| `top10_adjusted.with_column` | Thêm cột mới vào Table. | `top10_adjusted.with_column('Millions', millions)` | `top10_adjusted.with_column('Millions', millions)` |
| `top10_gross.barh` | Vẽ biểu đồ thanh ngang. | `top10_gross.barh('Title', 'Gross')` | `top10_gross.barh('Title', 'Gross')` |
| `top10_gross.column` | Lấy cột dữ liệu từ Table. | `top10_gross.column('Year')` | `top10_gross.column('Year')` |
| `top10_gross.with_column` | Thêm cột mới vào Table. | `top10_gross.with_column('Age', ages)` | `top10_gross.with_column('Age', ages)` |
| `top10_with_age.barh` | Vẽ biểu đồ thanh ngang. | `top10_with_age.barh('Title', 'Age')` | `top10_with_age.barh('Title', 'Age')` |
| `top_movies.bin` | Phương thức của đối tượng trong notebook. | `top_movies.bin('Age', bins = my_bins)` | `top_movies.bin('Age', bins = my_bins)` |
| `top_movies.column` | Lấy cột dữ liệu từ Table. | `top_movies.column('Year')` | `top_movies.column('Year')` |
| `top_movies.group` | Nhóm dữ liệu theo giá trị cột. | `top_movies.group('Studio')` | `top_movies.group('Studio')` |
| `top_movies.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `top_movies.hist('Age', bins = my_bins, unit = 'Year')` | `top_movies.hist('Age', bins = my_bins, unit = 'Year')` |
| `top_movies.select` | Chọn cột cần làm việc trong Table. | `top_movies.select('Title', 'Age')` | `top_movies.select('Title', 'Age')` |
| `top_movies.show` | Hiển thị nội dung Table. | `top_movies.show(6)` | `top_movies.show(6)` |
| `top_movies.sort` | Sắp xếp bảng theo cột. | `top_movies.sort('Gross', descending=True)` | `top_movies.sort('Gross', descending=True)` |
| `top_movies.take` | Lấy các hàng chỉ định theo chỉ số. | `top_movies.take(np.arange(10))` | `top_movies.take(np.arange(10))` |
| `top_movies.with_column` | Thêm cột mới vào Table. | `top_movies.with_column('Age', ages)` | `top_movies.with_column('Age', ages)` |
| `topkclasses.where` | Lọc dòng theo điều kiện. | `topkclasses.where('Class', are.equal_to(1))` | `topkclasses.where('Class', are.equal_to(1))` |
| `total_below_999.column` | Lấy cột dữ liệu từ Table. | `total_below_999.column('2019')` | `total_below_999.column('2019')` |
| `total_below_999.plot` | Vẽ biểu đồ từ Table dữ liệu. | `total_below_999.plot('AGE', 'Population (in millions)')` | `total_below_999.plot('AGE', 'Population (in millions)')` |
| `total_below_999.scatter` | Vẽ biểu đồ phân tán từ Table. | `total_below_999.scatter('AGE', 'Population (in millions)')` | `total_below_999.scatter('AGE', 'Population (in millions)')` |
| `total_below_999.with_columns` | Thêm nhiều cột mới vào Table. | `total_below_999.with_columns('Population (in millions)', total_below_999.column('2019')/1e6)` | `total_below_999.with_columns('Population (in millions)', total_below_999.column('2019')/1e6)` |
| `train.column` | Lấy cột dữ liệu từ Table. | `train.column('2nd Flr SF')` | `train.column('2nd Flr SF')` |
| `train.row` | Truy cập hàng trong Table hoặc tạo hàng mới. | `train.row(0)` | `train.row(0)` |
| `train.sample` | Lấy mẫu ngẫu nhiên từ Table. | `train.sample(with_replacement=False)` | `train.sample(with_replacement=False)` |
| `train.select` | Chọn cột cần làm việc trong Table. | `train.select('Class')` | `train.select('Class')` |
| `train.split` | Phương thức của đối tượng trong notebook. | `train.split(k = round(train.num_rows*(7/10)))` | `train.split(k = round(train.num_rows*(7/10)))` |
| `training.drop` | Xóa cột khỏi Table. | `training.drop(y_name)` | `training.drop(y_name)` |
| `training.scatter` | Vẽ biểu đồ phân tán từ Table. | `training.scatter('Hemoglobin', 'Glucose', group='Class')` | `training.scatter('Hemoglobin', 'Glucose', group='Class')` |
| `training.with_column` | Thêm cột mới vào Table. | `training.with_column('Distance', all_distances(training, new_point, y_name))` | `training.with_column('Distance', all_distances(training, new_point, y_name))` |
| `triple` | Hàm tự định nghĩa trong notebook. | `triple(np.arange(4))` | `triple(np.arange(4))` |
| `tvd` | Hàm tự định nghĩa trong notebook. | `tvd(sample_proportions(1453, model), jury.column('Eligible'))` | `tvd(sample_proportions(1453, model), jury.column('Eligible'))` |
| `two_cards_drawn.item` | Lấy giá trị đơn trong hàng/array. | `two_cards_drawn.item(1)` | `two_cards_drawn.item(1)` |
| `type` | Trả về kiểu dữ liệu của biến. | `type(nba)` | `type(nba)` |
| `united.column` | Lấy cột dữ liệu từ Table. | `united.column("Delay")` | `united.column("Delay")` |
| `united.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `united.hist('Delay', bins = delay_bins, unit = 'minute')` | `united.hist('Delay', bins = delay_bins, unit = 'minute')` |
| `united.sample` | Lấy mẫu ngẫu nhiên từ Table. | `united.sample(k=5, with_replacement=False)` | `united.sample(k=5, with_replacement=False)` |
| `united.show` | Hiển thị nội dung Table. | `united.show(6)` | `united.show(6)` |
| `united.take` | Lấy các hàng chỉ định theo chỉ số. | `united.take(np.arange(start, stop=start + 25, step=5))` | `united.take(np.arange(start, stop=start + 25, step=5))` |
| `united.where` | Lọc dòng theo điều kiện. | `united.where('Destination', 'JFK')` | `united.where('Destination', 'JFK')` |
| `united.with_column` | Thêm cột mới vào Table. | `united.with_column('Row', np.arange(united.num_rows))` | `united.with_column('Row', np.arange(united.num_rows))` |
| `urlopen` | Mở URL và đọc dữ liệu. | `urlopen(url)` | `urlopen(url)` |
| `us_pop.drop` | Xóa cột khỏi Table. | `us_pop.drop('2014')` | `us_pop.drop('2014')` |
| `us_pop.show` | Hiển thị nội dung Table. | `us_pop.show(5)` | `us_pop.show(5)` |
| `us_pop.where` | Lọc dòng theo điều kiện. | `us_pop.where('AGE',999)` | `us_pop.where('AGE',999)` |
| `us_pop_2019.show` | Hiển thị nội dung Table. | `us_pop_2019.show(3)` | `us_pop_2019.show(3)` |
| `us_pop_2019.where` | Lọc dòng theo điều kiện. | `us_pop_2019.where('AGE',are.below(999))` | `us_pop_2019.where('AGE',are.below(999))` |
| `us_women.scatter` | Vẽ biểu đồ phân tán từ Table. | `us_women.scatter('height')` | `us_women.scatter('height')` |
| `us_women.show` | Hiển thị nội dung Table. | `us_women.show(5)` | `us_women.show(5)` |
| `values_table.hist` | Vẽ biểu đồ histogram từ Table hoặc data. | `values_table.hist('value', bins = bins_for_display)` | `values_table.hist('value', bins = bins_for_display)` |
| `walk` | Hàm tự định nghĩa trong notebook. | `walk()` | `walk()` |
| `where` | Lọc dòng theo điều kiện. | `career.drop('Semester').where('Dept', 'Data')` | `career.drop('Semester').where('Dept', 'Data')` |
| `which_k` | Hàm tự định nghĩa trong notebook. | `which_k(new_train, 'Class', validation, k_s)` | `which_k(new_train, 'Class', validation, k_s)` |
| `with_averages.scatter` | Vẽ biểu đồ phân tán từ Table. | `with_averages.scatter('College%')` | `with_averages.scatter('College%')` |
| `with_column` | Thêm cột mới vào Table. | `Table().with_column(title, tvds)` | `Table().with_column(title, tvds)` |
| `with_columns` | Thêm nhiều cột mới vào Table. | `Table().with_columns([
    'Tom', np.char.count(huck_finn_chapters, 'Tom'),
    'Jim', np.char.count(huck_finn_chapters, 'Jim'),
    'Huck', np.char.count(huck_finn_chapters, 'Huck'),
])` | `Table().with_columns([
    'Tom', np.char.count(huck_finn_chapters, 'Tom'),
    'Jim', np.char.count(huck_finn_chapters, 'Jim'),
    'Huck', np.char.count(huck_finn_chapters, 'Huck'),
])` |
| `with_dists.sort` | Sắp xếp bảng theo cột. | `with_dists.sort('Distance')` | `with_dists.sort('Distance')` |
| `zero_one_pop.apply` | Phương thức của đối tượng trong notebook. | `zero_one_pop.apply(sd_of_zero_one_population, 'Number of Ones')` | `zero_one_pop.apply(sd_of_zero_one_population, 'Number of Ones')` |
| `zero_one_pop.scatter` | Vẽ biểu đồ phân tán từ Table. | `zero_one_pop.scatter('Proportion of Ones', 'Pop SD')` | `zero_one_pop.scatter('Proportion of Ones', 'Pop SD')` |
| `zero_one_pop.show` | Hiển thị nội dung Table. | `zero_one_pop.show()` | `zero_one_pop.show()` |
| `zero_one_pop.with_column` | Thêm cột mới vào Table. | `zero_one_pop.with_column('Pop SD', sds)` | `zero_one_pop.with_column('Pop SD', sds)` |
